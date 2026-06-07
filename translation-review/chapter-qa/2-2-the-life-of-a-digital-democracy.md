# 2-2 The Life of a Digital Democracy QA

## 요약 판정

전체적으로 원문 구조와 주요 논지를 잘 보존한 번역이다. Markdown heading 계층, 링크 URL, 이미지 경로, figure 구조, 각주 식별자는 모두 대응되며, code fence는 원문과 번역 모두 없다. 다만 스터디용 고품질 번역 기준에서는 통계 비교의 "비율" 표현, 모바일 추적 시스템, 마스크 앱의 정부 데이터 흐름, 동성혼 친족 예외 설명처럼 의미가 흐려진 곳을 우선 수정하는 편이 좋다. 그 밖에는 `Quadratic`, `information integrity`, `controlled substances` 등 핵심 용어의 장간 일관성 점검이 필요하다.

## P0 구조/누락

- 해당 없음. 원문 15개 heading과 번역 15개 heading이 모두 대응되며, 2개 figure 블록(`<figure>`, `<img>`, `<figcaption>`, `</figure>`, `<br></br>`), 이미지 URL/width, 링크 URL, 각주 참조/정의 목록이 보존되어 있다.

## P1 의미 오역

- [P1] 번역 74 / "harnessed data that the government ... to map mask availability" / "정부가 활용한 데이터를 사용해"는 시민 해커가 정부 공개 데이터를 활용했다는 흐름을 정부가 이미 쓰던 데이터를 재사용한 것처럼 흐린다 / "정부가 개방·투명 데이터 관행에 따라 공개한 데이터를 활용해 마스크 재고를 지도화했다"처럼 수정.
- [P1] 번역 76 / "phone-based social distancing and tracing systems" / "전화 기반"은 유선전화 또는 통화 기반처럼 읽혀 모바일 기반 추적·거리두기 시스템의 의미가 약해진다 / "휴대전화 기반" 또는 "스마트폰 기반 사회적 거리두기 및 추적 시스템"으로 수정.
- [P1] 번역 130 / "Differences in rates ... about 10 times as many Americans..." / "미국인은 ... 대만인보다 약 10배 많다"는 절대 인구 수 비교처럼 읽힐 수 있어 원문의 비율 비교가 흐려진다 / "매달 불법 약물을 쓴다고 보고한 미국인의 비율은, 불법 약물을 한 번이라도 시도해 본 대만인의 비율보다 약 10배 높다"로 수정.
- [P1] 번역 146 / "a legalization bill that exempted kin from the same-sex marriage process" / "친족을 면제하는 합법화 법안"은 친족이 무엇에서 면제되는지 불명확하고 제도 설계의 핵심이 약하다 / "동성혼 절차에서 친족에게 참여 의무나 법적 결속이 미치지 않도록 하는 합법화 법안"처럼 풀어 번역.

## P2 용어/문체

- [P2] 번역 26 / "a non-partisan, not-for-profit, grassroots movement" / g0v 선언문 핵심 정의가 영어 원문 그대로 남아 있다 / "비당파적·비영리 풀뿌리 운동"을 병기하거나 번역.
- [P2] 번역 60 / "The Public Digital Innovation Space (PDIS)" / 기관명이 영어로만 제시되어 스터디 독자가 기능을 즉시 파악하기 어렵다 / "공공디지털혁신공간(Public Digital Innovation Space, PDIS)"처럼 첫 등장 정의.
- [P2] 번역 62, 66, 68 / "quadratic signals", "Quadratic Voting", "Quadratic Voting to Funding" / "2차 신호/2차 투표/2차 펀딩"은 수학적 `quadratic`과 장기 용어가 불안정해 보인다 / 책 전체 용어집에 맞춰 "제곱 투표", "쿼드래틱 보팅", "제곱 신호" 중 하나로 통일.
- [P2] 번역 78, 80, 138 / "Information integrity" / "정보 무결성"은 직역으로 정확하나 허위정보 대응 맥락에서는 다소 기술 보안 용어처럼 읽힌다 / 장 전체 용어가 아니라면 "정보 신뢰성", "정보 생태계의 건전성" 등과 비교해 용어집 기준을 확정.
- [P2] 번역 82 / "more engagingly to rumors" / "더 관심을 끄는 방식"은 선정적 흥미 유발처럼 읽힐 수 있다 / "더 높은 참여를 유도하며" 또는 "더 상호작용적으로"로 수정.
- [P2] 번역 86 / "Line" / 메신저 서비스명이 "Line"으로 표기되어 공식 표기와 다르다 / "LINE"으로 통일.
- [P2] 번역 88 / "failed to polarize or noticeably sway the election" / "선거를 양극화하거나"는 대상이 어색하고 의미가 흔들린다 / "유권자/여론을 양극화하거나 선거 결과를 눈에 띄게 흔드는 데 실패했다"로 수정.
- [P2] 번역 126 / "fairly egalitarian" / "평등주의적"은 이념 성향처럼 들려 분배 상태 설명과 어긋난다 / "상당히 평등했거나" 또는 "분배가 비교적 평등했거나"로 수정.
- [P2] 번역 130 / "controlled substances" / "규제 약물"은 한국어 독자에게 법적 분류가 모호하다 / "통제 약물", "규제 대상 약물", 또는 맥락상 "마약류"로 조정.
- [P2] 번역 99 / "rights of compulsory sale" / "강제 매각권"만으로는 조세 장치와 결합된 권리라는 뜻이 딱딱하고 불명확하다 / "강제매각 청구권" 또는 "강제 매각을 요구할 권리"처럼 풀어 번역.
- [P2] 번역 100 / "Participation Officer Network" / "참여 담당관 네트워크"는 의미는 맞지만 대만 PDIS 맥락의 공식 제도명으로는 다소 일반명사화된다 / 다른 장 용어와 맞춰 "참여관 네트워크" 또는 "참여 담당관(PO) 네트워크" 병기 검토.

## P3 취향/윤문

- [P3] 번역 10 / "about human experience" / "인간 경험에 관한 것"은 시구의 리듬이 다소 설명문처럼 꺾인다 / "인간의 경험으로 만들자" 또는 "인간 경험의 문제로 만들자"처럼 운율 조정.
- [P3] 번역 20, 90 / "Illustrations", "Other programs" / "예시들", "다른 프로그램들"은 복수 접미사가 반복되어 다소 번역투다 / "사례", "기타 프로그램" 정도로 간결화.
- [P3] 번역 35 / "non-technical civil society groups" / "비기술 시민사회 단체"는 수식 관계가 뻣뻣하다 / "비기술 분야의 시민사회 단체" 또는 "기술자가 중심이 아닌 시민사회 단체"로 윤문.
- [P3] 번역 47 / "conventional microblogging services" / "전통적 마이크로블로깅 서비스"는 오래된 제도처럼 들린다 / "기존 마이크로블로깅 서비스"로 자연화.
- [P3] 번역 56 / "questions around technology regulation" / "기술 규제 관련 질문"은 정책 의제 문맥에서 딱딱하다 / "기술 규제를 둘러싼 쟁점"으로 수정.
- [P3] 번역 86 / "wagging his rear" / "엉덩이를 흔드는 자신의 사진"은 의미는 전달되지만 한국어 문장 안에서 갑작스럽고 거칠다 / "엉덩이를 흔드는 익살스러운 이미지"처럼 유머 맥락을 살림.
- [P3] 번역 132 / "Western and minority religions" / "서구 및 소수 종교"는 한 덩어리인지 병렬인지 모호하다 / "서구 종교와 소수 종교" 또는 "서구·소수 종교"로 수정.
- [P3] 번역 169 / "ailing Western democracies" / "병들어 가는 서구 민주주의"는 원문의 비판성을 살리지만 구어적 강도가 높다 / 스터디 문체에서는 "쇠약해지는 서구 민주주의"도 검토 가능.

## 권장 수정안

1. P1 네 항목을 먼저 반영해 핵심 사실관계와 통계 비교를 안정화한다.
2. `Quadratic`, `information integrity`, `controlled substances`, `Participation Officer`는 장 단위가 아니라 책 전체 용어집 기준으로 확정한다.
3. 첫 등장 기관명은 한국어 설명+영문 원명+약어 형식으로 맞추면 스터디 독자에게 더 친절하다.
4. 각주 문헌 제목을 번역할지 원문 유지할지 한 스타일로 정한다. 현재는 대체로 번역되어 있지만 일부 핵심 인용문은 영어가 남아 있다.

## 보류/주의

- 원문 91의 "fought of the pandemic"은 원문 오탈자로 보이며, 현재 번역의 "팬데믹을 막아냈듯"은 의미상 적절하다.
- 원문 각주 `[^demsupp]`의 "Taiwan Country Report Report" 중복은 원문 자체의 중복으로 보인다. 번역의 "대만 국가 보고서 보고서"는 어색하므로 최종 편집에서 원문 충실성과 문헌명 정리 원칙 중 어느 쪽을 우선할지 결정해야 한다.
- `Plurality`를 "플루럴리티"로 음역한 것은 가능하지만, 책 전체에서 "다원성/플루럴리티" 병기 여부가 정해져 있다면 그 기준을 따라야 한다.
