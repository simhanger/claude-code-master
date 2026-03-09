# 계획: 개인 프로필 웹사이트 생성

## Context
사용자가 HTML + CSS + JavaScript + Tailwind CSS CDN으로 개인 프로필 웹사이트 생성을 요청.
- 디자인 스타일: **다크 모드** (어두운 배경, 밝은 텍스트)
- 콘텐츠: 샘플 데이터로 시작 → 나중에 직접 수정 가능하도록 주석 포함
- 반응형 레이아웃, 모던 & 깔끔한 UI

---

## 파일 구조

```
/Users/musinsa/study/ai/claude-code-mastery/
└── profile/
    └── index.html   ← 단일 파일 (HTML + Tailwind CDN + inline JS)
```

---

## 페이지 섹션 구성

| 섹션 | 내용 |
|------|------|
| **Hero** | 이름, 직업/역할, 짧은 슬로건, CTA 버튼 |
| **About** | 자기소개 2~3줄 |
| **Skills** | 기술 스택 배지 형태 표시 |
| **Projects** | 카드 3개 (제목, 설명, 기술 태그, 링크) |
| **Contact** | 이메일, GitHub 링크 |
| **Footer** | 저작권 |

---

## 샘플 데이터

- **이름**: 홍길동
- **역할**: 풀스택 개발자 (Full-Stack Developer)
- **소개**: 사용자 경험을 중심으로 생각하는 개발자입니다. Java와 JavaScript를 기반으로 다양한 웹 서비스를 개발해왔으며, 클린 코드와 효율적인 아키텍처에 관심이 많습니다.
- **기술 스택**: Java, Spring Boot, JavaScript, React, HTML/CSS, Tailwind CSS, Git
- **프로젝트 3개**: 샘플 포트폴리오 카드 (제목 / 설명 / GitHub 링크)
- **연락처**: example@email.com / github.com/username

---

## 디자인 사양

- **배경**: `bg-gray-900` (매우 어두운 회색)
- **카드 배경**: `bg-gray-800`
- **강조 색상**: Tailwind `indigo-500` / `indigo-400` (파란-보라 계열)
- **텍스트**: `text-white` / `text-gray-300`
- **폰트**: `Inter` (Google Fonts CDN)
- **애니메이션**: 스크롤 fade-in 효과 (Intersection Observer API)
- **반응형**: Tailwind 반응형 클래스 (`sm:`, `md:`, `lg:`)

---

## 기술 구현 방식

1. **Tailwind CSS**: CDN 방식 (`<script src="https://cdn.tailwindcss.com">`)
2. **JavaScript (inline)**:
   - 네비게이션 스크롤 하이라이트
   - 스크롤 시 섹션 fade-in 애니메이션 (Intersection Observer)
   - 모바일 메뉴 토글
3. **단일 HTML 파일**: 외부 의존성 최소화

---

## 생성 대상 파일

- `profile/index.html` (신규 생성) — HTML + Tailwind CDN + inline JS 포함

---

## 검증

1. 브라우저에서 `profile/index.html` 파일을 열어 렌더링 확인
2. 각 섹션(Hero, About, Skills, Projects, Contact) 표시 확인
3. 모바일 크기(375px)에서 반응형 확인
4. 스크롤 애니메이션 동작 확인
