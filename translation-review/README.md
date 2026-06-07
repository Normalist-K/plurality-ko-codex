# Plurality 한국어 번역 v0.2 리뷰

이 디렉터리는 `contents/korean/`의 Codex 자동 번역본을 스터디용으로 개선하기 위해 만든 공개 QA 산출물이다. 공식 한국어 번역 승인본이나 출판 품질 원고가 아니며, 사람 검수를 대체하지 않는다.

## 방식

- 원문 `contents/english/`와 번역문 `contents/korean/`을 장별로 대조했다.
- 장별 리포트는 누락, 오역, 의미 약화/과잉, 용어 불일치, 한국어 문체, 제목/소제목, 각주/참고문헌, Markdown 구조를 같은 기준으로 확인했다.
- severity는 `P0 구조/누락`, `P1 의미 오역`, `P2 용어/문체`, `P3 취향/윤문`으로 나눴다.
- 수정은 리포트에서 확인된 항목만 반영하며, heading, 링크 URL, 이미지 경로, code fence, figure 구조는 보존한다.

## 현재 범위

- 장별 QA 리포트: 36/36개
- 구조 baseline: 36개 확인, 누락 0개, 구조 mismatch 0개
- 기준 용어: `Plurality=플루럴리티`, `⿻` 유지, `deliberation=숙의`, `quadratic voting=2차 투표`, `quadratic funding=2차 펀딩`, `social markets=사회적 시장`

## 파일

- `qa-summary.md`: 전체 이슈 요약과 완료/보류 현황
- `chapter-qa/`: 장별 한영 대조 QA 리포트
- `revision-log.md`: 실제 번역문에 반영한 수정 기록

## 한계

- 이번 라운드는 Codex 자동 QA/편집만 사용했다.
- 공식 한국어 작업자, Discord 번역 채널, 원저자 측과 아직 조율하지 않았다.
- 참고문헌/고유명사/링크 현지화 정책은 보수적으로 유지했다.
