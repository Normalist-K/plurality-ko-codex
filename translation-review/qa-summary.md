# v0.2 QA Summary

Plurality 한국어 번역 v0.2 품질 개선 라운드의 장별 한영 대조 결과를 집계했다.

## Baseline

- 한국어 Markdown 파일: 36/36개 확인
- 누락 파일: 0개
- heading/link/image/code fence/figure count mismatch: 0개
- 기존 구조 QA 기준: `84 pass / 3 warn / 0 fail`, 구조 검증 이슈 0개

## Issue Counts

- P0 구조/누락: 2개
- P1 의미 오역: 40개
- P2 용어/문체: 262개
- P3 취향/윤문: 209개

## Chapter Status

| file | report | P0 | P1 | P2 | P3 |
| --- | --- | ---: | ---: | ---: | ---: |
| `0-0-endorsements.md` | done | 0 | 0 | 9 | 6 |
| `0-1-About-the-authors.md` | done | 0 | 1 | 3 | 2 |
| `0-2-finding-your-dao.md` | done | 0 | 0 | 5 | 6 |
| `0-3-credits.md` | done | 0 | 1 | 3 | 2 |
| `1-preface.md` | done | 0 | 0 | 5 | 5 |
| `2-0-information-technology-and-democracy-a-widening-gulf.md` | done | 0 | 4 | 9 | 5 |
| `2-1-a-view-from-yushan.md` | done | 0 | 2 | 9 | 8 |
| `2-2-the-life-of-a-digital-democracy.md` | done | 0 | 4 | 11 | 8 |
| `3-0-what-is-⿻.md` | done | 0 | 2 | 6 | 4 |
| `3-1-living-in-a-⿻-world.md` | done | 0 | 2 | 8 | 7 |
| `3-2-connected-society.md` | done | 0 | 1 | 8 | 8 |
| `3-3-the-lost-dao.md` | done | 0 | 1 | 6 | 4 |
| `4-0-rights-os-and-⿻-freedom.md` | done | 0 | 1 | 8 | 6 |
| `4-1-identity-and-personhood.md` | done | 0 | 2 | 8 | 7 |
| `4-2-association-and-⿻-publics.md` | done | 0 | 1 | 10 | 5 |
| `4-3-commerce-and-trust.md` | done | 0 | 3 | 10 | 10 |
| `4-4-property-and-contract.md` | done | 0 | 3 | 7 | 4 |
| `4-5-access.md` | done | 0 | 0 | 8 | 5 |
| `5-0-collaborative-technology-and-democracy.md` | done | 0 | 1 | 6 | 4 |
| `5-1-post-symbolic-communication.md` | done | 0 | 0 | 7 | 5 |
| `5-2-immersive-shared-reality.md` | done | 0 | 1 | 5 | 5 |
| `5-3-creative-collaborations.md` | done | 0 | 1 | 7 | 5 |
| `5-4-augmented-deliberation.md` | done | 2 | 1 | 6 | 6 |
| `5-5-adaptive-administration.md` | done | 0 | 1 | 8 | 6 |
| `5-6-⿻-voting.md` | done | 0 | 0 | 8 | 9 |
| `5-7-social-markets.md` | done | 0 | 1 | 7 | 5 |
| `6-0-from-⿻-to-reality.md` | done | 0 | 1 | 9 | 8 |
| `6-1-workplace.md` | done | 0 | 1 | 9 | 5 |
| `6-2-health.md` | done | 0 | 2 | 8 | 9 |
| `6-3-media.md` | done | 0 | 1 | 7 | 7 |
| `6-4-environment.md` | done | 0 | 0 | 8 | 8 |
| `6-5-learning.md` | done | 0 | 1 | 9 | 6 |
| `7-0-policy.md` | done | 0 | 0 | 9 | 6 |
| `7-1-conclusion.md` | done | 0 | 0 | 9 | 6 |
| `8-blurb.md` | done | 0 | 0 | 5 | 5 |
| `Plurality Book Ownership List.md` | done | 0 | 0 | 2 | 2 |

## Cross-Cutting Checks

- `cross-qa/structure-baseline.md`: 36개 파일의 heading/link/image/code fence/figure count baseline.
- `cross-qa/english-residue.md`: URL/Markdown 링크를 제외한 영어 잔존량 스캔. 참고문헌, 인명, 기관명은 자동 수정 대상이 아니다.
- `cross-qa/heading-map.md`: 원문 제목과 한국어 제목 대응표.
- `cross-qa/terminology-scan.md`: 핵심 용어 후보의 기계적 일관성 스캔.

## Fixed / Deferred

- Fixed: P0 구조/누락 2개, P1 의미 오역 40개를 `contents/korean/`에 반영했다.
- Deferred: P2 용어/문체 262개, P3 취향/윤문 209개는 장별 QA 리포트에 남기고 이번 라운드에서는 본문 반영을 보류했다.
- Remaining P0/P1: 0개. 단, 이는 Codex 자동 QA 기준이며 사람 검수 결과를 의미하지 않는다.

## Remaining Risk

- 자동 QA는 장별 의미 대조와 P0/P1 수정 반영을 수행했지만 사람 번역가의 문체 감수와 사실 검증을 대체하지 않는다.
- 참고문헌과 고유명사 표기 정책은 공식 번역 조율이 생기면 재검토해야 한다.
