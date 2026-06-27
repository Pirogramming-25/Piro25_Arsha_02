# Piro25_Arsha_02 — Arsha 클론코딩

> HTML/CSS만 사용한 Arsha 페이지 반응형 클론코딩 (JS·외부 라이브러리 사용 금지)
> 원본: https://bootstrapmade.com/demo/Arsha/

## 👥 팀원 & 역할 분담
| 이름 | 담당 섹션 |
| --- | --- |
| 신은아 | Header, Hero  |
| 정현민 | About, Why Us / Skills, Services  |
| 이수빈 | Work Process, Call To Action, Portfolio  |
| 문예지 | Team, Pricing, Testimonials|
| 강보민 | FAQ, Subscribe, Recent Blog, Contact, Footer  |



### 전체 섹션 순서 (위 → 아래, 총 16개)
1. Header  2. Hero  3. About  4. Why Us/Skills  5. Services
6. Work Process  7. Call To Action  8. Portfolio  9. Team  10. Pricing
11. Testimonials  12. FAQ  13. Subscribe  14. Recent Blog  15. Contact  16. Footer

## 📐 코드 컨벤션
- 클래스 이름: 소문자 + 하이픈 (`hero-section`, `pricing-card`)
- 이름은 모양❌ 역할⭕ (`blue-box`❌ → `pricing-card`⭕)
- 들여쓰기: 스페이스 2칸
- CSS 단위: rem 기본, 작은 값은 px 허용
- 색상은 공통 변수 사용, 직접 색코드 작성 금지
- 디자인은 class 사용 (id 자제)

## 🎨 공통 CSS 변수 (css/style.css 맨 위)
\`\`\`css
:root {
  --accent: #47b2e4;     /* 메인 파란색 */
  --dark: #37423b;       /* 진한 텍스트 */
  --gray: #5e5e5e;       /* 본문 회색 */
  --bg-light: #f6f9fe;   /* 연한 배경 */
  --font: "Open Sans", sans-serif;
}
\`\`\`
> 정확한 색은 원본에서 F12로 확인 후 보정

## 📁 폴더 구조
\`\`\`
Piro25_Arsha_02/
├── index.html
├── css/
│   ├── style.css      (공통: 변수·리셋·폰트)
│   └── (섹션별).css    (header.css, hero.css ...)
└── images/
\`\`\`
- 공통(변수·리셋)은 style.css에
- 각 섹션 CSS는 자기 파일에 작성 (충돌 방지)

## 🌿 브랜치 전략
- `main` : 최종 완성본 (직접 커밋 금지)
- `feature/섹션명` : 각자 작업 브랜치 (예: `feature/header`)
- 작업 완료 → PR 올리기 → 리뷰 후 머지

## ✍️ 커밋 메시지 컨벤션
형식: `타입: 내용`
- `feat:` 기능/섹션 구현 — `feat: 헤더 네비게이션 구현`
- `fix:` 버그·오류 수정 — `fix: 푸터 정렬 깨짐 수정`
- `style:` 디자인·CSS 수정 — `style: 버튼 호버 효과 추가`
- `docs:` 문서 수정 — `docs: 역할분담 표 업데이트`

## ⚠️ 주의사항 (과제 규칙)
- ❌ JS 사용 금지 / ❌ Bootstrap·jQuery·Swiper·AOS 등 외부 라이브러리 금지
- 반응형 웹 필수 (모바일 화면 대응)
- Portfolio 필터 · Testimonials 슬라이드는 CSS만으로 구현
- Recent Blog 카드 클릭 → 디테일 이동은 구현 X
