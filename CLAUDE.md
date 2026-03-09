# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 언어 및 커뮤니케이션 규칙

- **기본 응답 언어**: 한국어
- **코드 주석**: 한국어로 작성
- **커밋 메시지**: 한국어로 작성
- **문서화**: 한국어로 작성
- **변수명/함수명**: 영어 (코드 표준 준수)

## 프로젝트 개요

Claude Code의 다양한 기능(슬래시 명령어, MCP, 훅, 에이전트 등)을 학습하고 실습하기 위한 프로젝트.

- **주요 언어**: Java 21, HTML/CSS/JavaScript
- **IDE**: IntelliJ IDEA
- **JDK**: homebrew-21
- **Git 원격**: https://github.com/simhanger/claude-code-master.git

## 프로젝트 구조

```
claude-code-mastery/
├── profile/
│   └── index.html        # 개인 포트폴리오 웹사이트 (Tailwind CSS CDN + inline JS)
├── study.txt             # Claude Code 학습 노트
└── .claude/
    ├── settings.json     # plans 디렉토리 설정
    └── plans/            # 계획 파일 저장 위치
```

### profile/index.html

단일 HTML 파일로 구성된 반응형 포트폴리오 사이트:
- **섹션**: Hero, About, Skills, Projects, Contact, Footer
- **스타일**: Tailwind CSS CDN + 커스텀 CSS (inline)
- **기능**: 스크롤 fade-in (Intersection Observer), 모바일 메뉴 토글, 네비게이션 활성 상태
- **확인 방법**: 브라우저에서 `profile/index.html` 직접 열기

## 빌드 및 실행

빌드 도구가 추가되면 아래에 명령어를 기록합니다.

- **Maven 사용 시**: `mvn compile`, `mvn test`, `mvn test -Dtest=TestClassName`
- **Gradle 사용 시**: `./gradlew build`, `./gradlew test`, `./gradlew test --tests "패키지.클래스명"`

컴파일 출력 디렉토리: `out/` (IntelliJ 기본 설정)

## 개발 환경 확인

```bash
java -version  # Java 21 확인
```
