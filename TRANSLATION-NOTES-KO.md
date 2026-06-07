# 한국어 자동 번역 작업 노트

## 범위

- 대상 원본: `contents/english/*.md`
- 산출 위치: `contents/korean/*.md`
- 파일 수: 36
- 생성 시각: `2026-06-07T03:01:53.457916+00:00`
- 원본 commit: `1c0f160e7858251677c0982a56518bb404d3dc21`

## 품질 상태

- 자동 QA: `84` pass / `3` warn / `0` fail
- 구조 검증 이슈: `0`
- v0.2 Codex 장별 QA/편집: 36개 장별 한영 대조 리포트 작성, P0 `2`건과 P1 `40`건 반영, P2/P3는 보류

## 운영 원칙

1. 이 저장소는 원본 프로젝트에 PR하지 않는 개인/스터디 공유용 fork로 둔다.
2. 번역 문장은 자동 생성 초안으로 표시하고, 공식 한국어판처럼 보이는 표현을 피한다.
3. 추후 품질을 올리고 싶으면 장별로 사람 검수 commit을 쌓는다.
4. 공식 `plurality.net` 웹사이트에 반영하려면 별도의 웹사이트 레포 작업과 승인 절차가 필요하다.

## 1. Codex 멀티 에이전트 번역 워크플로

이번 번역은 메인 Codex가 전체 작업을 오케스트레이션하고, 다수의 하위 worker가 chunk 단위 번역과 편집을 맡는 rolling pipeline 방식으로 진행했다. 메인 Codex는 직접 번역량을 크게 떠안기보다 원문 분석, chunk 분할, manifest 생성, worker 배정, QA 실행, 누락 확인, 최종 조립을 담당했다.

작업 단위는 `contents/english/*.md` 36개 파일을 기준으로 만들었다. 원문은 보수적 집계 기준 약 151,362 words, 1,032,271 characters였고, chunk 목표 크기는 약 2,300 words, 최대 2,600 words로 잡았다. 그 결과 총 87개 chunk가 생성되었다.

하위 worker는 크게 두 종류로 운용했다.

- Translator worker: `work/translation/chunks/.../*.source.md`를 읽고 `work/translation/translated/.../*.ko.md`에 1차 번역을 작성했다.
- Editor worker: 번역본을 자연스럽게 다듬고 용어를 맞춘 뒤 `work/translation/edited/.../*.ko.md`에 최종 후보를 작성했다.

충돌 방지를 위해 worker는 자신에게 배정된 출력 파일만 쓰도록 했다. `manifest.jsonl`, QA 실행, 최종 장별 Markdown 조립은 메인 Codex가 관리했다. 최종 `contents/korean/*.md`에 해당하는 장별 산출물은 worker가 직접 만들지 않고, integration 단계에서만 생성했다.

공유 상태판 역할은 `work/translation_state/manifest.jsonl`이 맡았다. 각 항목에는 source hash, chunk 번호, source/translated/edited/qa 경로, 진행 상태와 QA 상태가 기록되었다. 별도의 worker inbox 문서는 저장소에 남기지 않았지만, manifest와 `work/translation/*` 디렉터리 규약이 실질적인 멀티 에이전트 공유문서 역할을 했다.

실행 중 동시 활성 worker 한도는 대략 6개로 확인되었다. 이후에는 번역 worker 약 3개와 편집 worker 약 3개를 유지하며, worker가 완료되면 메인 Codex가 결과를 회수하고 해당 worker를 닫은 뒤 다음 chunk를 새 worker에게 배정하는 방식으로 진행했다. 초기 계획상 전체 subagent job 수는 번역, 편집, QA, 재작업, 조립을 합쳐 약 175-205개로 예상했다.

QA는 `work/scripts/qa_translation_outputs.py`로 수행했다. 검사 항목은 Markdown heading, 링크 URL, 이미지 URL, code fence, figure 수, 모델 메타 문구, 과도한 영어 잔존, 지나치게 짧은 출력 등이었다. QA를 통과하거나 warning만 남은 edited chunk만 장별 조립 대상으로 삼았다.

## 2. 실제 Codex 작업 로그

실제 실행은 먼저 10개 chunk pilot batch로 시작했다. 프론트매터와 2-0 초반 chunk를 translator worker에게 나누어 맡겼고, 첫 QA에서 9개 pass, 1개 fail이 나왔다. fail 원인은 번역 품질 문제가 아니라 `About the authors`의 링크 URL 순서 불일치였다. 메인 Codex가 해당 링크 순서를 원문과 맞게 보정한 뒤 pilot batch는 모두 QA를 통과했다.

pilot 이후에는 번역과 편집을 겹쳐 돌렸다. Part 2를 끝까지 번역하면서 동시에 첫 batch를 editor worker에게 넘겼고, 이후 Part 3, Part 4, Part 5, Part 6, Part 7, 부속 파일 순서로 rolling pipeline을 이어갔다. 큰 장은 여러 chunk로 나누어 배정했다. 예를 들어 2-0은 6개 chunk, 3-3은 5개 chunk, 7-0은 4개 chunk로 처리했다.

중간 QA에서 영어 잔존 warning이 과하게 발생했다. 원인은 URL 안의 영어 단어까지 영어 잔존율 계산에 포함했기 때문이었다. 이에 따라 QA 스크립트를 수정해 URL을 제외하고 영어 잔존율을 계산하도록 보정했다.

작업 후반에는 `assemble_korean_auto.py`를 추가해 edited chunk를 장별 Markdown으로 조립할 준비를 했다. 마지막 QA에서 missing 2개가 발견되었고, 확인 결과 6-1과 6-2의 짧은 마지막 chunk가 번역 라인에서 누락된 것이었다. 두 chunk는 마지막 worker에게 번역과 편집 파일 생성을 함께 맡겨 누락을 닫았다.

최종 QA 결과는 총 87개 chunk 중 84 pass, 3 warn, 0 fail이었다. 남은 warning 3개는 주로 참고문헌과 각주에 남은 영어 고유명, 논문 제목, 기관명 때문에 발생했다. 구조 파손이나 누락은 발견되지 않았다.

마지막으로 `assemble_korean_auto.py`가 87개 edited chunk를 36개 장별 Markdown으로 조립했고, `verify_assembled_outputs.py`가 원문 대비 heading/link/image/code fence/figure 구조 보존을 검증했다. 최종 조립본 검증 이슈는 `0`개였다.

## 3. v0.2 Codex 장별 QA/편집 라운드

v0.2 라운드는 `리포트 후 수정` 원칙으로 진행했다. 먼저 36개 한국어 Markdown 전체에 대해 장별 한영 대조 QA 리포트를 만들고, 그 리포트에서 확인된 P0/P1 항목만 `contents/korean/`에 반영했다.

장별 QA는 36개 worker가 각 장의 원문 전체와 번역문 전체를 대조하는 방식으로 수행했다. 리포트 항목은 누락, 오역, 의미 약화/과잉, 용어 불일치, 한국어 문체, 제목/소제목, 각주/참고문헌, Markdown 구조로 고정했다. severity는 `P0 구조/누락`, `P1 의미 오역`, `P2 용어/문체`, `P3 취향/윤문`으로 나누었다.

교차 검증으로는 구조 baseline, 영어 잔존, 제목 대응, 용어 일관성 스캔을 수행했다. 구조 기준은 원문 대비 heading, link, image, code fence, figure count가 모두 일치해야 한다는 보수적 기준을 사용했다.

편집 단계에서는 5개 편집 worker가 P0/P1이 있는 25개 파일의 full-file 후보를 만들고, 1개 worker가 P0/P1이 없는 11개 파일을 수정 없음으로 확인했다. 메인 Codex는 후보 파일 구조를 다시 검증한 뒤 fork의 `contents/korean/`에 통합했다.

최종 반영 범위는 P0 `2`건, P1 `40`건이다. P2 `262`건과 P3 `209`건은 대량 윤문으로 번지지 않도록 이번 라운드에서는 보류하고, `translation-review/chapter-qa/`와 `translation-review/revision-log.md`에 추적 가능한 형태로 남겼다.

## 포함 파일

- `0-0-endorsements.md`
- `0-1-About-the-authors.md`
- `0-2-finding-your-dao.md`
- `0-3-credits.md`
- `1-preface.md`
- `2-0-information-technology-and-democracy-a-widening-gulf.md`
- `2-1-a-view-from-yushan.md`
- `2-2-the-life-of-a-digital-democracy.md`
- `3-0-what-is-⿻.md`
- `3-1-living-in-a-⿻-world.md`
- `3-2-connected-society.md`
- `3-3-the-lost-dao.md`
- `4-0-rights-os-and-⿻-freedom.md`
- `4-1-identity-and-personhood.md`
- `4-2-association-and-⿻-publics.md`
- `4-3-commerce-and-trust.md`
- `4-4-property-and-contract.md`
- `4-5-access.md`
- `5-0-collaborative-technology-and-democracy.md`
- `5-1-post-symbolic-communication.md`
- `5-2-immersive-shared-reality.md`
- `5-3-creative-collaborations.md`
- `5-4-augmented-deliberation.md`
- `5-5-adaptive-administration.md`
- `5-6-⿻-voting.md`
- `5-7-social-markets.md`
- `6-0-from-⿻-to-reality.md`
- `6-1-workplace.md`
- `6-2-health.md`
- `6-3-media.md`
- `6-4-environment.md`
- `6-5-learning.md`
- `7-0-policy.md`
- `7-1-conclusion.md`
- `8-blurb.md`
- `Plurality Book Ownership List.md`
