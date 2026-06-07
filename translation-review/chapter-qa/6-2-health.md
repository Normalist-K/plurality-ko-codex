# 6-2-health QA

## 요약 판정

스터디용으로 전반적으로 양호한 번역이다. 장 전체의 논지, 문단 순서, 번호 목록, bullet 목록, 각주 라벨, 링크 URL, 이미지 경로, `<figure>`/`<img>`/`<figcaption>`/`<br></br>` 구조가 보존되어 있으며, code fence는 원문과 번역 모두 없다. 치명적 누락이나 구조 붕괴는 보이지 않는다. 다만 후반부의 GFM/원주민 보건 행정 문단에서 주체가 살짝 바뀌는 의미 문제가 있고, `impact`, `health agency`, `extitutional`, `confounded` 등 핵심 용어는 장 전체 및 한국어판 용어표에 맞춰 정리할 필요가 있다.

## P0 구조/누락

해당 없음.

- 구조 확인: H1 1개와 `###` heading 6개가 모두 대응한다.
- 구조 확인: 도입부 구분선 `---`, 번호 목록 2개, 마지막 bullet 목록 1개가 모두 보존되어 있다.
- 구조 확인: Figure 6-2-A/B의 이미지 URL, `width="100%"`, `alt`, figcaption, figure 닫힘 태그, `<br></br>`가 모두 보존되어 있다.
- 구조 확인: 링크 URL은 원문과 번역이 동일하다.
- 구조 확인: 각주 호출/정의 라벨과 개수는 원문과 번역이 일치한다.
- 구조 확인: 원문과 번역 모두 code fence가 없다.

## P1 의미 오역

- [P1] `보건 협력을 위한 숙의 도구` 마지막 문장/`whose "synthetic wisdom" can be queried..., or who can be tasked with designing...`/현재 번역은 과제를 맡는 주체가 `"합성 지혜"`처럼 읽혀, 원문의 가상적 `"individual"`이 질의되고 설계를 맡을 수 있다는 구조가 흐려짐/`그러한 "개인"의 "합성 지혜"를 실시간으로 질의하거나, 그 "개인"에게 비식민주의적 모델에 따른 인센티브 양립적 의료와 개입 설계를 맡길 수 있다`처럼 주체를 복원.
- [P1] `보건 협력을 위한 숙의 도구` 원주민 보건 행정 문단/`redesigning, systems of healthcare administration to be more responsive to cultural value systems`/현재 `의료 행정 시스템을 문화적 가치 체계에 더 민감하게 해석하고, 비판하고...`는 `more responsive`가 해석·비판에도 걸려 시스템을 재설계한다는 목적 관계가 어색해짐/`의료 행정 시스템을 해석·비판·재상상하고, 궁극적으로 문화적 가치 체계에 더 잘 반응하도록 재설계`로 조정.

## P2 용어/문체

- [P2] 도입부 핵심 개념/`health agency`/현재 `건강 행위주체성`은 의미는 통하지만 다소 조어 느낌이 강함/한국어판 용어표가 없다면 `건강 주체성`, `건강 행위능력`, `건강 행위주체성` 중 하나를 정하고 각주·본문에서 일관 적용.
- [P2] `건강보험 다시 상상하기`/`risk smoothing`/현재 `위험 완충`은 뜻은 전달되지만 보험 맥락의 시간적 변동 완화가 약함/`위험 평탄화`, `위험 변동 완화`, `위험의 시간적 완화` 등으로 검토.
- [P2] `건강보험 다시 상상하기`/`infections and globally transmissible diseases`/현재 `감염 및 전 세계적으로 전파되는 질병`은 `infections`가 질병 범주가 아니라 행위/상태처럼 읽힘/`감염병 및 말라리아, HIV, 결핵처럼 전 지구적으로 전파될 수 있는 질병`으로 정리.
- [P2] `보건 임팩트 토큰화`/`outputs`, `outcomes`, `impacts`/heading은 `임팩트`, 본문 정의는 `영향`으로 나뉘어 핵심 3분법이 덜 선명함/`산출물`, `성과`, `임팩트(영향)`처럼 첫 정의에서 병기한 뒤 장 내 용어를 통일.
- [P2] `보건 임팩트 토큰화` 번호 목록 2번/`subscription to pools`/현재 `풀 가입`은 금융적 출자·참여의 뉘앙스가 약하고 일반 회원가입처럼 들림/`풀 참여/출자/청약을 위한 열린 조율 표준` 등 맥락에 맞춰 조정.
- [P2] `공평한 편익 공유에 인센티브 부여하기`/`pooled mechanisms for the prepayment`/현재 `공동 부담 메커니즘`은 risk pooling의 제도적 의미가 약함/`공동화된 선납 메커니즘` 또는 `위험을 공동화해 선납하는 메커니즘` 검토.
- [P2] `보건 협력을 위한 숙의 도구`/`extitutional`/현재 `외부제도적(extitutional)`은 뜻을 짐작하기 어렵고 기존 `institutional`과의 대비가 흐림/책 전체 용어와 맞춰 `외제도적`, `탈제도적`, `확장제도적` 중 하나를 정하고 원어 병기.
- [P2] `진단과 치료를 지원하는 GFMs와 데이터 공유`/`confounded signals`/현재 `교란된 신호`는 신호 자체가 망가진 듯 들림/역학·통계 맥락을 살려 `교란 요인이 많이 섞인 신호` 또는 `강하게 교란된 신호`로 수정.

## P3 취향/윤문

- [P3] `건강보험 다시 상상하기`/`the Scandinavian countries ... have smaller populations than most large private health insurers in the US`/현재 `민간 건강보험사 대부분보다 인구가 적다`는 보험사의 `인구`라는 표현이 어색함/`가입자 수가 더 적다` 또는 `포괄하는 인구가 더 적다`로 윤문.
- [P3] `건강보험 다시 상상하기`/`collectivized contributions`/현재 `공동화된 기여금`은 의미는 맞지만 딱딱함/`공동 부담 기여금` 또는 `집합적으로 부담하는 기여금` 검토.
- [P3] `건강보험 다시 상상하기`/`the full host of technologies`/현재 `온갖 기술`은 구어적이고 다소 과장되어 보임/`앞서 설명한 일련의 기술들`로 차분하게 정리.
- [P3] `보건 임팩트 토큰화`/`open-source commodity`, `forked`/현재 `오픈소스 재화`, `포크`는 기술 독자에게는 자연스럽지만 일반 스터디 독자에게는 은유가 거칠 수 있음/첫 등장에 `오픈소스 상품/재화`, `분기해 활용`처럼 풀어쓰기 검토.
- [P3] `보건 협력을 위한 숙의 도구`/`would have multiplied by orders of magnitude`/현재 `몇 자릿수 배가했을 것`은 직역투가 강함/`몇 배수의 규모로 증폭했을 것`, `수십 배 이상 키웠을 것` 등으로 자연화.
- [P3] `보건을 위한 탈상징적 커뮤니케이션`/`The usual operating system is that of the sensory and motor organs`/현재 `일반적인 운영체제`는 컴퓨터 은유를 살리지만 약간 뜬금없음/`일반적인 작동 체계는 감각기관과 운동기관이다`로 완화.
- [P3] `보건을 위한 탈상징적 커뮤니케이션`/`non-interpersonal medical settings`/현재 `비대인적 의료 환경`은 전문어처럼 보이나 잘 굳은 표현은 아님/`대인 상호작용이 중심이 아닌 의료 환경`으로 풀어쓰기.
- [P3] `보건을 위한 탈상징적 커뮤니케이션`/`simulated and non-simulated social interaction`/현재 `시뮬레이션된, 그리고 시뮬레이션되지 않은 사회적 상호작용`은 직역투가 강함/`시뮬레이션 기반 및 실제 사회적 상호작용`으로 윤문.
- [P3] Web2/Web3 문단/`open-ended contingent liability`/현재 `기한 없는 우발채무`는 법률·회계 용어 느낌이 강해 독자가 건강 데이터 위험을 바로 잡기 어려울 수 있음/`끝을 알 수 없는 잠재적 프라이버시 책임/위험`처럼 의미 중심으로 풀어쓰기.

## 권장 수정안

1. P1 두 곳을 먼저 수정한다. 두 항목 모두 문장 구조상의 주체·목적 관계 문제라, 스터디 독자의 이해에 직접 영향을 준다.
2. 핵심 용어는 `health agency`, `impact`, `outcome`, `output`, `risk pooling`, `risk smoothing`, `extitutional`, `confounded` 순으로 용어표를 고정한 뒤 장 전체에 일괄 적용한다.
3. 링크 URL, 이미지 URL, figure 태그, 각주 라벨은 현재 잘 보존되어 있으므로 번역 수정 시 구조 요소를 건드리지 않는다.
4. 기술 은유(`open-source`, `fork`, `operating system`)는 원문의 맛을 남기되, 첫 등장에서는 한국어 풀이를 조금 보태 스터디용 가독성을 높인다.

## 보류/주의

- `radiographer`를 현재 `방사선사`로 옮긴 것은 원문 직역으로는 타당하다. 다만 문맥상 `view and interpret`가 영상 판독 행위를 가리키므로 한국 의료 제도 관점에서는 `영상의학 판독자/전문의`가 더 자연스러울 수 있다. 원문 의도 확인 전에는 보류.
- 원문 `Global Fund to AIDS, Tuberculosis and Malaria`는 통상 명칭 `Global Fund to Fight AIDS, Tuberculosis and Malaria`와 다르게 쓰여 있다. 번역은 `퇴치를 위한 글로벌 펀드`로 자연화했지만, 원문 오탈자 가능성이 있어 번역만 따로 문제 삼기보다는 편집 방침 확인이 필요하다.
- 일부 장 제목 링크 텍스트는 한국어로 번역되어 있고 일부는 `Augmented Deliberation`, `Post-Symbolic Communication`처럼 영어로 남아 있다. 장 전체/책 전체 링크 제목 표기 정책이 정해진 뒤 일괄 정리하는 편이 안전하다.

이슈 개수: P0 0개, P1 2개, P2 8개, P3 9개.
