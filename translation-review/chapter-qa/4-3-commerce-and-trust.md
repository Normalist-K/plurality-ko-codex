# 4-3-commerce-and-trust QA

## 요약 판정

전체 구조와 주요 의미 흐름은 양호하게 보존되어 있어 스터디용으로 읽을 수 있는 번역이다. 다만 금융/신뢰/정체성 논의의 핵심 동사가 명사처럼 처리되거나, 일부 관계 구문이 뒤집힌 곳이 있어 P1 수정이 필요하다. 용어 면에서는 `identity`, `obligation`, `private`, `social currency`, `submodular/supermodular` 계열을 장 전체와 시리즈 전체 기준으로 맞추면 품질이 더 안정된다.

Markdown heading, 링크 URL, 이미지 경로, figure 구조는 보존되어 있다. 원문과 번역 모두 167줄이며, `###` heading 5개, `<figure>`/`<img>`/`</figure>`/`<br></br>` 구조가 같은 위치에 있다. code fence는 원문/번역 모두 없다. 각주 정의도 누락 없이 대응한다.

## P0 구조/누락

- 없음. 장 제목, 절 제목, 구분선, 번호 목록, figure, 이미지 URL, figcaption, `<br></br>`, 각주 정의는 모두 보존됨.

## P1 의미 오역

- [P1] 102행/`The decline of cash, heralded by defenders...`/현재 번역은 `예고한 현금의 쇠퇴`로 처리해 제재 체제 옹호자와 금융범죄 대응론자가 현금 쇠퇴를 예측했다는 뜻에 가깝다/문맥상 `bemoaned by`와 대비되는 `환영받은`, `반긴`, `긍정적으로 받아들인` 쪽으로 수정.
- [P1] 117행/`the community services of a hunter for a village or an elder`/현재 번역은 `마을이나 원로를 위해 사냥꾼이 제공한`으로 읽혀 원로가 봉사의 수혜자가 된다/`마을의 사냥꾼이나 원로가 공동체에 제공한 봉사`처럼 사냥꾼 또는 원로가 공동체에 기여한 구조로 수정.
- [P1] 158행/`Identity systems are about trusting/credit claims made by someone about a third party`/현재 번역 `신뢰/신용 주장을 믿거나 인정`은 신뢰와 신용 자체에 대한 주장처럼 읽힌다/`누군가가 제3자에 대해 한 주장을 신뢰하거나 신용하는 문제`처럼 `trusting/crediting claims`의 동작을 살려 수정.

## P2 용어/문체

- [P2] 39행/`government identities`/현재 번역 `정부가 부여한 정체성`은 한국어에서 개인의 정체성을 정부가 부여한다는 뉘앙스가 강하다/결제 인프라 맥락에서는 `정부 발급 신원`, `공적 신원 인증`, `정부 신원 체계` 등으로 조정.
- [P2] 53행/`directed transfers`, `undirected value transfers`/현재 번역 `방향이 지정되지 않은 가치 이전`은 직역감이 강하고 금융 의미가 흐리다/`수취인 지정 이체`, `무기명 또는 비지정 가치 이전`처럼 결제 용어로 정리.
- [P2] 92행/`obligations`/현재 번역 `_의무_`는 일반 윤리적 의무처럼 읽힐 수 있다/상거래·회계 맥락에서는 `_채무_`, `_부채 관계_`, 필요시 `의무/채무` 병기로 수정.
- [P2] 96행/`private, rapid and low-cost processors`/현재 번역 `사적이고 빠르며 저비용인 처리 업체`는 privacy의 `private`처럼 오해될 수 있다/`민간의 빠른 저비용 결제 처리업체`로 수정.
- [P2] 102행/`highly private currencies`/현재 번역 `고도로 사적인 통화`는 어색하고 의미가 흐리다/`강한 프라이버시를 보장하는 통화`, `프라이버시 특화 암호화폐`로 수정.
- [P2] 113행/`lending circles`/현재 번역 `대출 모임`은 제도적·상호부조적 함의가 약하다/`상호부조 금융 모임`, `대출계`, `소액 신용 모임` 등으로 문맥화.
- [P2] 131-133행/`submodular`, `supermodular`/현재 번역이 `서브모듈러`와 `초모듈적`으로 혼재한다/`서브모듈러/슈퍼모듈러` 또는 `부분모듈적/초모듈적` 중 하나로 일관.
- [P2] 137행/`advertising against ... the person holding the prestige`/현재 번역 `그 명망을 지닌 사람과 연결해 광고`는 원문의 상업적 전환 방식을 다소 흐린다/`그 명망에 기대어 광고를 붙이거나`, `그 명망을 광고 지면/맥락으로 활용하거나`처럼 수정.
- [P2] 150행/`social currencies (of likes, friends, network centrality, citations, etc.)`/현재 번역 `사회적 통화`는 실제 화폐로 좁게 읽힐 수 있다/`사회적 화폐`, `사회적 평판 지표`, 필요시 `사회적 통화/화폐` 병기 검토.
- [P2] 154행/`internet working committees`/현재 번역 `인터넷 워킹 위원회`는 일반 워킹그룹처럼 보인다/표준화·네트워크 프로토콜 맥락을 살려 `인터넷워킹 위원회`, `인터넷 표준 작업 위원회` 등으로 조정.

## P3 취향/윤문

- [P3] 19행/`His warm smile was contagious`/현재 번역 `전염성이 있었다`는 의미는 맞지만 다소 직역투다/`그의 따뜻한 미소는 절로 따라 웃게 했다`처럼 자연스럽게 윤문.
- [P3] 27행/`acknowledging his recent help...`/현재 번역이 `인정하는 내용이었다`로 문장이 끊겨 설명문처럼 느껴진다/앞문장에 붙여 `... 이모지가 나타나며, 최근 공동체 프로젝트를 도운 일을 알아봐 주고 있었다`처럼 조정.
- [P3] 61행/`recognizably modern credit card`/현재 번역 `알아볼 수 있을 만큼 현대적인 신용카드`가 부자연스럽다/`오늘날의 신용카드로 알아볼 수 있는 형태의 최초 성공 사례`로 윤문.
- [P3] 67행/`[^Swift].`/현재 번역도 `[^Swift].`로 마침표가 중복되어 보인다/원문 오탈자 보존 원칙과 별개로 한국어판에서는 `[^Swift]` 뒤 중복 마침표 제거 검토.
- [P3] 123행/`money as a solvent in socially long-distance trust`/현재 번역 `매개물로 작동하는 돈의 역할`은 `solvent`의 은유가 약하다/`사회적으로 먼 신뢰 관계를 이어 주는 용매/매개 장치로서의 돈`처럼 은유를 약하게 보강.
- [P3] 127행/`such shorthand`/현재 번역 `그러한 약식 표기`는 기호학적 표현처럼 보인다/`그런 간편한 증표`, `그런 축약적 매개물` 등으로 자연화.
- [P3] 129행/`far more plausible civic or political leader`/현재 번역 `훨씬 더 그럴듯한`은 구어적이다/`훨씬 더 설득력 있는`, `훨씬 더 적합한`으로 조정.
- [P3] 145행/각주 URL 뒤 공백/현재 번역 `plural-money/ 를 보라`처럼 URL과 조사 사이 공백이 있다/Markdown 자동 링크 안정성을 고려한 의도일 수 있으나, 표기 통일 기준에 따라 유지 또는 괄호 처리 검토.
- [P3] 148행/`creation of this book`/현재 번역 `이 책의 창작`은 문학 작품처럼 들린다/공동 집필 맥락에서는 `이 책의 작성`, `이 책의 제작`이 더 자연스럽다.
- [P3] 158행/`industries[^AfricaInnovation] even as ... gaps[^IdentificationAfrica]`/현재 번역은 두 각주가 문장 끝에 붙어 출처 대응이 덜 선명하다/`핀테크 산업을 선도했다[^AfricaInnovation]. 대륙이 ... 공백과 씨름하는 가운데서도 말이다[^IdentificationAfrica].`처럼 각주 위치를 원문 의미 단위에 가깝게 조정 검토.

## 권장 수정안

- 102행: `현금의 쇠퇴는 ... 예고한`보다 `현금의 쇠퇴는 ... 환영받아 왔지만`으로 바꾸면 `privacy advocates ... bemoaned`와 대비가 살아난다.
- 117행: `마을이나 원로를 위해 사냥꾼이 제공한 공동체적 봉사`는 `마을의 사냥꾼이나 원로가 공동체에 제공한 봉사`로 수정하는 것을 권장한다.
- 158행: `정체성 시스템은 누군가가 제3자에 대해 한 주장을 신뢰하거나 신용하는 문제이다`처럼 고치면 문장의 논리와 다음 공격 가능성 설명이 자연스럽게 이어진다.
- 장 전체: `identity`는 `정체성`을 기본으로 유지하되 정부 발급 신원·인증 맥락에서는 `신원`, `신원 체계`를 쓰고, `obligation/debt/credit`은 각각 `채무/부채`, `부채`, `신용`으로 용어표를 세우는 것이 좋다.

## 보류/주의

- 원문 자체에 `identitifiers`, `transaction".[^Swift].`, `commercial trust systems systems`처럼 보이는 오탈자 또는 중복 표현이 있다. 번역에서 조용히 정리할지 원문 보존 원칙을 따를지는 편집 기준 확인이 필요하다.
- 영화 제목 `Rogue Stardust`, `Whispers in the Void`, `The Last Alchemist`와 고유 서비스명은 현재 원문 유지되어 있으며 문제로 보지 않았다.
- figure의 `alt`와 figcaption은 번역되어 있고 이미지 URL은 원문과 동일하다. `public domain`을 번역할지는 전체 판본 표기 관례에 맞추면 된다.
- 링크 URL과 각주 라벨은 누락 없이 보존되어 있다. 다만 158행 마지막 문장의 각주 위치는 의미 단위 대응을 위해 조정 여지가 있다.
