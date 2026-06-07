# 4-1 Identity and Personhood QA

## 요약 판정

스터디용 번역으로는 전반적으로 사용 가능하다. 장 구조, 소제목 5개, 수평선, 목록, 각주 식별자, 링크 URL은 원문과 대응하며, 원문/번역 모두 이미지 경로, code fence, figure 구조는 없다. 큰 구조 누락은 없지만, 다중심성 논의에서 `players`를 `참여자`로 옮겨 검증자 수 제한이라는 논지가 흐려지는 대목은 우선 수정이 필요하다. 그 외에는 SSO/DID/VC/KYC 등 전문 용어의 일관성과 일부 직역투를 정리하면 품질이 더 좋아진다.

## P0 구조/누락

없음.

## P1 의미 오역

- [P1] 번역 174행 / 원문 단서 `The polycentric approach tries to manage this problem by limiting the number of players.` / 현재 `참여자의 수를 제한`으로 옮겨, 뒤이어 말하는 검증자·발급자 규모 제한 논리가 개인 참여자 수 제한처럼 읽힘 / `행위자 수`, 문맥상 더 명확히 `검증자 수` 또는 `검증 주체 수`로 수정.
- [P1] 번역 147행 / 원문 단서 `some combination of people and institutions (typically many) who can "vouch"` / 현재 `어떤 조합(대개는 여러 조합)`은 “다수의 보증 주체”가 아니라 “여러 조합”이 있다는 뜻으로 기울어짐 / `정보를 보증해 줄 수 있는 사람과 기관의 조합, 대개 다수의 주체`처럼 redundancy의 의미를 살림.

## P2 용어/문체

- [P2] 번역 61행 / 원문 단서 `Social Security for pensions and taxes in the US` / 현재 `Social Security`가 그대로 남아 식별번호 맥락이 약함 / `미국의 연금·세금용 사회보장번호(SSN)`처럼 후속 SSN 논의와 연결.
- [P2] 번역 73행 / 원문 단서 `single sign-on (SSO)` / 현재 `single sign-on`, `SSO`, `단일 로그인`이 한 문단에 섞임 / 첫 출현을 `싱글 사인온(single sign-on, SSO)` 또는 `단일 로그인(SSO)`으로 정하고 이후 통일.
- [P2] 번역 73행 / 원문 단서 `the identity provider` / 현재 `정체성 제공자`는 직역에 가까움 / 기술 용어로 `신원 제공자(IdP)`를 쓰거나, 장 전체 용어집이 `정체성`을 채택한다면 `정체성 제공자(IdP)`처럼 약어를 병기.
- [P2] 번역 84행 / 원문 단서 `know your customer or KYC` / 현재 `고객 알기`는 한국어 금융·인증 문맥에서 어색함 / `고객확인(KYC)` 또는 `고객확인제도(KYC)`로 수정.
- [P2] 번역 84행 / 원문 단서 `portability across private providers` / 현재 `민간 제공자 사이에서 ... 이동성`은 의미가 흐림 / `민간 제공자 사이의 이전 가능성` 또는 `이식성`으로 수정.
- [P2] 번역 98행, 131행 / 원문 단서 `Verifiable Credentials`, `verifiable credentials` / 현재 98행은 영문 그대로, 131행은 `검증 가능 자격증명`으로 처리되어 불일치 / 첫 출현에서 `검증 가능 자격증명(Verifiable Credentials, VC)`로 병기하고 이후 통일.
- [P2] 번역 127행 / 원문 단서 `globally resolvable endpoints` / 현재 `전 지구적으로 해석 가능한 엔드포인트`는 DID의 resolver 뉘앙스가 약함 / `전 지구적으로 확인 가능한 엔드포인트` 또는 `전역적으로 해소 가능한 엔드포인트` 등으로 조정.
- [P2] 번역 150행 / 원문 단서 `AI and printing technology` / 현재 `AI와 프린팅 기술`은 일반 독자에게 기술 범위가 좁게 느껴질 수 있음 / `AI와 인쇄 기술`로 자연화.

## P3 취향/윤문

- [P3] 번역 3행 / 원문 단서 `In the swiftly moving line` / 현재 `줄이 빠르게 움직이는 가운데`는 대기열 장면이 다소 물리적으로 들림 / `빠르게 줄어드는 대기열 속에서` 또는 `대기줄이 빠르게 앞으로 나아가는 가운데`로 윤문.
- [P3] 번역 19행 / 원문 단서 `immortalized in a digital shield of recognition` / 현재 `인정의 디지털 방패 속에 영구히 기록`은 은유가 딱딱함 / `디지털 인정 기록 속에 오래 남아`처럼 의미를 유지하며 완화.
- [P3] 번역 69행 / 원문 단서 `backstopped by arduous legal procedures` / 현재 `고된 법적 절차에 의해 뒷받침`은 직역투 / `끝내는 까다로운 법적 절차가 받쳐 주는 경우가 많다`로 자연화.
- [P3] 번역 71행 / 원문 단서 `volatile mix`, `unattractive trade-off` / 현재 `불안정한 혼합물`, `매력적이지 않은 절충`은 의미는 맞지만 어색함 / `위험한 조합`, `불리한 절충` 정도로 조정.
- [P3] 번역 93행 / 원문 단서 `real-life connections` / 현재 `실제 생활 연결`은 어색함 / `현실 세계의 관계` 또는 `오프라인 관계`로 수정.
- [P3] 번역 114행 / 원문 단서 `globally universal biometric identity` / 현재 `전 지구적 보편 생체 정체성`은 개념어가 뭉침 / `전 지구적으로 보편적인 생체 신원 시스템`처럼 풀어 쓰기.
- [P3] 번역 120행 / 원문 단서 `eyeballs can ... be spoofed` / 현재 `눈을 위조할 수`는 다소 부자연스러움 / `안구/홍채 인증을 속일 수`로 조정.

## 권장 수정안

우선순위는 P1 두 건을 먼저 반영한 뒤, 용어 표준화를 한 번에 적용하는 방식이 좋다. 특히 `identity`, `digital identity`, `identity provider`, `Verifiable Credentials`, `DID`, `KYC`, `portability`는 이 장 안에서만이 아니라 앞뒤 장과 맞춰야 하므로 용어집 기준을 확인해 일괄 조정하는 편이 안전하다. 이후 P3 항목은 본문 의미를 바꾸지 않는 선에서 낭독감과 스터디 가독성을 높이는 윤문으로 처리하면 된다.

## 보류/주의

- 원문 134행의 `single issue`는 문맥상 `single issuer` 오탈자로 보이며, 번역은 `단일 발급자`로 합리적으로 보정했다. 원문 보존 원칙이 엄격하다면 편집자 확인 권장.
- 원문 152행의 `work, play or workshop`은 `worship` 또는 다른 단어의 오탈자 가능성이 있으나, 현재 번역은 원문 그대로 `워크숍`을 따르고 있어 확정 이슈로 분류하지 않았다.
- 원문 자체에 일부 URL 뒤 문장부호가 붙어 추출되는 곳이 있으나, 번역도 동일하게 보존되어 구조적 문제로 보지는 않았다.
