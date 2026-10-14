# 개발자 웹 이력서 ROADMAP

HTML, CSS, JavaScript, Tailwind CSS로 만드는 단일 페이지 개발자 이력서 사이트 개발 로드맵입니다.

## 1. 프로젝트 개요

- **목표**: 방문자가 한 페이지에서 나의 소개, 기술, 경력, 프로젝트, 연락처를 빠르게 확인할 수 있는 반응형 웹 이력서
- **기술스택**: HTML5, CSS3, JavaScript (ES6+), Tailwind CSS (CDN 또는 CLI)
- **배포**: GitHub Pages (또는 Netlify / Vercel)
- **원칙**: 프레임워크 없이 가볍게, 모바일 우선, 접근성 준수

## 2. 이력서 콘텐츠 (샘플)

| 섹션 | 내용 |
|------|------|
| Hero | 이름, 직무(예: 프론트엔드 개발자), 한 줄 소개, 연락 버튼 |
| About | 3~4줄 자기소개, 프로필 사진 |
| Skills | HTML/CSS, JavaScript, Tailwind CSS, Git, React 등 (숙련도 표시) |
| Experience | 회사명 / 직책 / 기간 / 주요 업무 2~3개 |
| Projects | 프로젝트 카드 3개 (설명, 사용 기술, 링크) |
| Education | 학교, 전공, 기간 |
| Contact | 이메일, GitHub, LinkedIn, 이력서 PDF 다운로드 |

> 모든 내용은 `홍길동` 등 더미 데이터로 먼저 작성한 후 실제 정보로 교체합니다.

## 3. 폴더 구조

```
resume/
├── index.html
├── css/
│   └── style.css        # Tailwind로 처리하기 어려운 커스텀 스타일
├── js/
│   └── main.js          # 인터랙션 (스크롤, 다크모드, 메뉴)
├── assets/
│   ├── images/          # 프로필, 프로젝트 썸네일
│   └── resume.pdf
└── ROADMAP.md
```

## 4. 개발 단계

### Phase 1. 환경 설정 (0.5일)
- [ ] 프로젝트 폴더 및 `index.html` 생성
- [ ] Tailwind CSS 연결 (CDN 방식으로 시작, 필요 시 CLI 전환)
- [ ] Tailwind 커스텀 설정 (폰트, 컬러 팔레트)
- [ ] Git 저장소 초기화

### Phase 2. 레이아웃 & 마크업 (1일)
- [ ] 시맨틱 태그로 구조 작성 (`header`, `nav`, `main`, `section`, `footer`)
- [ ] 섹션별 더미 콘텐츠 입력
- [ ] 네비게이션 바 (섹션 앵커 링크)

### Phase 3. 스타일링 (1~2일)
- [ ] Tailwind 유틸리티로 각 섹션 디자인
- [ ] 반응형 대응 (`sm`, `md`, `lg` 브레이크포인트)
- [ ] 스킬 카드, 프로젝트 카드, 경력 타임라인 컴포넌트화
- [ ] 호버/포커스 효과 및 트랜지션

### Phase 4. JavaScript 인터랙션 (1일)
- [ ] 모바일 햄버거 메뉴 토글
- [ ] 부드러운 스크롤 및 현재 섹션 네비게이션 하이라이트
- [ ] 스크롤 시 섹션 등장 애니메이션 (IntersectionObserver)
- [ ] 다크모드 토글 (`localStorage` 저장)
- [ ] 스킬 숙련도 바 애니메이션
- [ ] (선택) 연락 폼 유효성 검사

### Phase 5. 품질 개선 (0.5~1일)
- [ ] 접근성: alt 텍스트, 명도 대비, 키보드 탐색
- [ ] SEO: `title`, `meta description`, Open Graph 태그
- [ ] 이미지 최적화 (WebP, `loading="lazy"`)
- [ ] Lighthouse 점수 90+ 목표
- [ ] 크로스 브라우저 / 모바일 실기기 테스트
- [ ] 인쇄용 스타일 (`@media print`)

### Phase 6. 배포 (0.5일)
- [ ] GitHub Pages 또는 Netlify에 배포
- [ ] 커스텀 도메인 연결 (선택)
- [ ] 실제 이력서 정보로 콘텐츠 교체

## 5. 일정 요약

| 단계 | 기간 |
|------|------|
| Phase 1. 환경 설정 | 0.5일 |
| Phase 2. 레이아웃 & 마크업 | 1일 |
| Phase 3. 스타일링 | 1~2일 |
| Phase 4. JS 인터랙션 | 1일 |
| Phase 5. 품질 개선 | 0.5~1일 |
| Phase 6. 배포 | 0.5일 |
| **합계** | **약 4.5~6일** |

## 6. 완료 기준 (Definition of Done)

- 모바일/태블릿/데스크톱에서 레이아웃이 깨지지 않는다.
- 모든 섹션이 네비게이션으로 이동 가능하다.
- Lighthouse 성능/접근성/SEO 점수 90 이상
- 배포된 URL로 누구나 접속 가능하다.

## 7. 향후 확장 아이디어

- 다국어 지원 (한국어/영어 전환)
- 블로그 또는 포트폴리오 상세 페이지
- 방문자 통계 (Google Analytics 등)
- 스킬/프로젝트 데이터를 JSON으로 분리하여 JS로 렌더링
