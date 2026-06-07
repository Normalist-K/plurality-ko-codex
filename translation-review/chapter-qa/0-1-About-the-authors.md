# 0-1-About-the-authors QA

## 요약 판정

조건부 통과. 원문과 번역문 모두 8행이며, 이미지 2개, 링크 URL, `<br></br>`, `<span aria-label="Plurality">⿻</span>` 구조가 보존되어 있다. 원문에 Markdown heading, code fence, figure 블록은 없으며 누락도 없다. 다만 Audrey Tang 소개에서 직함의 소속/현재형이 약간 틀어지고, 일부 병렬 구조와 설명 문장이 스터디용 번역으로는 더 명확해질 수 있다.

## P0 구조/누락

- 없음.

## P1 의미 오역

- [P1] 3행 / "the inaugural Minister of Digital Affairs in 🇹🇼" / 현재 번역은 "초대 디지털부 장관으로 대만에서 일했으며"라서 직함이 '대만의 초대 디지털부 장관'이라는 점과 원문의 현재형 "is"가 약해짐 / "대만의 초대 디지털부 장관이며"처럼 직함과 현재성을 직접 살리는 방향 권장.

## P2 용어/문체

- [P2] 3행 / "Founder of RadicalxChange, Microsoft Research's Plural Technology Collaboratory & Plurality Institute" / 현재 번역은 "Microsoft Research의 ... 및 Plurality Institute의 창립자" 구조가 다소 압축되어 Plurality Institute의 소속 관계가 모호하게 읽힐 수 있음 / "RadicalxChange의 창립자이자, Microsoft Research의 Plural Technology Collaboratory 창립자이며, Plurality Institute의 창립자"처럼 병렬을 명확히 하는 방향 권장.
- [P2] 3행 / "the inaugural 🏳️‍⚧️ minister in the 🌐" / 현재 번역 "🌐 최초의 🏳️‍⚧️ 장관"은 의미와 링크는 보존하지만 한국어 독자에게 해독성이 낮음 / 원문의 이모지 감각을 살리되 "세계 최초의 [🏳️‍⚧️](https://en.wikipedia.org/wiki/List_of_transgender_political_office-holders) 장관" 또는 "세계 최초의 [트랜스젠더](https://en.wikipedia.org/wiki/List_of_transgender_political_office-holders) 장관" 검토.
- [P2] 8행 / "governed according to the principles described in this book by this community" / 현재 번역 "이 커뮤니티가 이 책에서 설명한 원칙에 따라 운영할 것이다"는 온라인판이 커뮤니티에 의해 거버넌스된다는 수동/관리 뉘앙스가 다소 약함 / "이 커뮤니티에 의해, 이 책에서 설명한 원칙에 따라 운영되며 계속 진화할 것이다"처럼 조정 권장.

## P3 취향/윤문

- [P3] 8행 / "open-source ... freely copied" / 현재 "오픈소스", "복사"는 이해 가능하지만 출판물 맥락에서는 약간 소프트웨어식/직역식으로 들림 / 필요하면 "오픈소스"는 유지하되 "자유롭게 복제·공유할 수 있다"처럼 독자 친화적으로 윤문.
- [P3] 8행 / "machine-generated blending of their faces, tiled by their individual faces" / 현재 "각자의 얼굴 타일로 구성된 이 기계 생성 합성 얼굴 이미지"는 의미를 보존하지만 길고 딱딱함 / "각자의 얼굴을 타일처럼 배열해 기계적으로 합성한 이 이미지"처럼 더 자연스럽게 다듬는 방향 검토.

## 권장 수정안

- 3행 Audrey Tang 문장: "[Audrey Tang](https://en.wikipedia.org/wiki/Audrey_Tang)은 [🇹🇼](https://en.wikipedia.org/wiki/Taiwan)의 초대 [디지털부 장관](https://en.wikipedia.org/wiki/Ministry_of_Digital_Affairs_%28Taiwan%29)이며, 세계 최초의 [🏳️‍⚧️](https://en.wikipedia.org/wiki/List_of_transgender_political_office-holders) 장관이다."
- 8행 마지막 문장: "[https://www.plurality.net/](https://www.plurality.net/)에서 제공되는 이 책의 무료 온라인판은 이 커뮤니티에 의해, 이 책에서 설명한 원칙에 따라 운영되며 계속 진화할 것이다."

## 보류/주의

- "🏳️‍⚧️", "🌐", "🇹🇼" 같은 이모지는 원문의 장난스럽고 압축적인 저자 소개 톤을 이루므로, 가독성을 위해 풀어 쓰더라도 링크와 상징성을 의도적으로 보존할지 번역 기준을 맞출 필요가 있다.
- 원문의 첫 저자 소개 문장은 `&`로 여러 소속과 역할을 빠르게 병렬 연결한다. 한국어에서는 쉼표와 "및"만으로 처리하면 소속 관계가 흔들릴 수 있으므로, 최종 번역 시 병렬 단위를 확인하는 것이 좋다.
