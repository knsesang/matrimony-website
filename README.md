# 인연맺음 - 소개 웹사이트

AI 기반 결혼중개 플랫폼 "인연맺음"의 공식 소개 웹사이트입니다.

## 🌐 라이브 사이트

**배포 예정:** Netlify를 통한 영구 배포

## 🚀 기술 스택

- **프레임워크:** SvelteKit
- **빌드 도구:** Vite
- **UI 라이브러리:** Svelte
- **스타일:** CSS-in-JS (Svelte)
- **배포:** Netlify

## 📋 프로젝트 구조

```
website/
├── src/
│   ├── main.js                 # 진입점
│   ├── App.svelte              # 메인 컴포넌트
│   └── components/
│       ├── Header.svelte       # 헤더
│       ├── Hero.svelte         # 히어로 섹션
│       ├── Features.svelte     # 특징
│       ├── Architecture.svelte # 아키텍처
│       ├── Technology.svelte   # 기술 스택
│       ├── Roadmap.svelte      # 로드맵
│       ├── Contact.svelte      # 문의
│       └── Footer.svelte       # 푸터
├── index.html                  # HTML 진입점
├── vite.config.js              # Vite 설정
├── netlify.toml                # Netlify 설정
├── package.json                # 의존성
└── dist/                       # 빌드 결과
```

## 🎨 웹사이트 섹션

### 1. Header
- 로고 및 타이틀
- 반응형 네비게이션 메뉴
- 스티키 포지셔닝

### 2. Hero
- 메인 타이틀
- 설명 텍스트
- CTA 버튼
- 통계 (30+ API, 7 테이블, 100% 오픈소스)

### 3. Features
6개의 핵심 특징:
- 🤖 AI 기반 매칭
- 🏢 운영위원 주도형
- 🔐 신뢰성 높은 인증
- 📱 모바일 우선 설계
- ⚡ 트래픽 분산
- 🌍 확장 가능성

### 4. Architecture
- 시스템 아키텍처 다이어그램
- 운영위원 VPS 구성
- 중앙 서버 구성

### 5. Technology
- 백엔드 기술 스택
- 배포 & 인프라
- 프론트엔드 기술
- API 통계

### 6. Roadmap
5단계 개발 계획:
1. Phase 1: 백엔드 기초 (완료)
2. Phase 2: 프론트엔드 개발 (진행 중)
3. Phase 3: AI 자동화 (계획)
4. Phase 4: 운영 고도화 (계획)
5. Phase 5: 확장 (계획)

### 7. Contact
- 문의 폼
- 연락처 정보
- 소셜 미디어 링크

### 8. Footer
- 회사 정보
- 링크 모음
- 저작권 정보

## 🛠️ 개발 가이드

### 설치

```bash
npm install
```

### 개발 서버 실행

```bash
npm run dev
```

브라우저에서 `http://localhost:5173` 접속

### 빌드

```bash
npm run build
```

`dist/` 폴더에 정적 파일 생성

### 프로덕션 미리보기

```bash
npm run preview
```

브라우저에서 `http://localhost:4173` 접속

## 📦 빌드 크기

| 항목 | 크기 |
|:-----|:-----|
| HTML | 0.49 KB |
| CSS | 14.01 KB |
| JavaScript | 38.32 KB |
| **전체** | **53 KB** |
| **gzip 압축** | **15 KB** |

## 🚀 배포

### Netlify 배포

1. GitHub에 저장소 푸시
2. Netlify.com 가입
3. "New site from Git" 클릭
4. GitHub 저장소 선택
5. 자동 배포 완료

**환경 변수:**
```
NETLIFY_AUTH_TOKEN=your_token
NETLIFY_SITE_ID=your_site_id
```

### 로컬 배포 테스트

```bash
npm run build
npm run preview
```

## 🔒 보안 기능

- ✅ X-Frame-Options (클릭재킹 방지)
- ✅ X-Content-Type-Options (MIME 스니핑 방지)
- ✅ X-XSS-Protection (XSS 방지)
- ✅ Referrer-Policy (리퍼러 제어)
- ✅ Permissions-Policy (기능 제한)

## 📱 반응형 디자인

- ✅ 모바일 (< 768px)
- ✅ 태블릿 (768px - 1024px)
- ✅ 데스크톱 (> 1024px)

## 🎨 디자인 특징

- **색상:** 보라색 (#667eea), 핑크 (#e91e63)
- **폰트:** 시스템 기본 폰트 (빠른 로딩)
- **애니메이션:** 부드러운 트랜지션
- **레이아웃:** 카드 기반, 그리드 시스템

## 📊 성능 최적화

- ✅ 정적 파일 배포
- ✅ gzip 압축
- ✅ 캐시 제어
- ✅ 이미지 최적화
- ✅ 번들 최소화

## 🔍 SEO

- ✅ 메타 태그
- ✅ 구조화된 콘텐츠
- ✅ 시맨틱 HTML
- ✅ 모바일 친화적

## 📝 라이선스

MIT License

## 👨‍💻 개발자

**Manus AI**

## 📞 문의

- 이메일: info@matrimony.com
- 전화: +82-2-1234-5678
- GitHub: [저장소 링크]

## 🙏 감사의 말

- SvelteKit 팀
- Vite 팀
- Netlify 팀

---

**마지막 업데이트:** 2025년 10월 24일
**버전:** 1.0.0

