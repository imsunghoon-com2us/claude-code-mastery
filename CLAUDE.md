# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 언어 및 커뮤니케이션 규칙

- **기본 응답 언어**: 한국어
- **코드 주석**: 한국어로 작성
- **커밋 메시지**: 한국어로 작성
- **문서화**: 한국어로 작성
- **변수명/함수명**: 영어 (코드 표준 준수)

## 프로젝트 개요

HTML, CSS, JavaScript, Tailwind CSS로 만드는 단일 페이지 개발자 웹 이력서입니다. 프레임워크 없이 가볍게 구성하며, 모바일 우선 반응형과 접근성을 지향합니다. 현재는 `ROADMAP.md`(개발 로드맵)만 존재하고 구현은 시작 전입니다.

## 현재 상태 및 명령어

- 빌드 시스템, 린터, 테스트가 아직 설정되어 있지 않습니다. 설정이 추가되면 이 섹션에 명령어를 기록하세요.
- Tailwind는 CDN 방식으로 시작하고, 필요할 때 CLI로 전환하는 것이 로드맵의 계획입니다.

## 계획된 구조 (`ROADMAP.md` 기준)

작업 전에 `ROADMAP.md`의 Phase별 체크리스트를 먼저 확인하고, 완료한 항목은 체크 표시로 갱신합니다.

- `index.html`: 시맨틱 태그(`header`, `nav`, `main`, `section`, `footer`)로 구성한 단일 페이지. 섹션은 Hero, About, Skills, Experience, Projects, Education, Contact.
- `css/style.css`: Tailwind 유틸리티로 처리하기 어려운 커스텀 스타일만 작성
- `js/main.js`: 모바일 메뉴, 스크롤 하이라이트, IntersectionObserver 애니메이션, 다크모드(`localStorage` 저장)
- `assets/`: 이미지와 `resume.pdf`

콘텐츠는 `홍길동` 등 더미 데이터로 먼저 작성하고, 마지막 단계에서 실제 정보로 교체합니다.
