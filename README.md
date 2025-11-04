# Olly Client

Next.js 프로젝트를 구성하기 위한 초기 템플릿입니다.

## 기술 스택

### Core

- **Node 버전**: 22.19.0
- **Next.js**: 15.5.6 (Turbopack 지원)
- **React**: 19.1.0
- **TailwindCSS**: ^4
- **TypeScript**: ^5

## 폰트

해당 템플릿에는 **Pretendard** 폰트가 적용되어 있습니다.

- 위치: `src/shared/assets/fonts/Pretendard/Pretendard.css`
- 전역 적용: `globals.css`를 통해 모든 요소에 기본 폰트로 설정

## 시작하기

### 필수 요구사항

- Node.js 22.19.0 이상

### 설치

```bash
# 의존성 패키지 설치
yarn install
```

### 개발 서버 실행

```bash
# 개발 모드 실행 (Turbopack 사용)
yarn dev
```

개발 서버가 실행되면 [http://localhost:3000](http://localhost:3000)에서 확인할 수 있습니다.

### 빌드

```bash
# 프로덕션 빌드 (Turbopack 사용)
yarn build
```

### 프로덕션 서버 실행

```bash
# 빌드 후 프로덕션 서버 실행
yarn start
```

## 프로젝트 구조

app router 적용

FSD 기반

해당 템플릿은 app, shared 만 작성

```
olly-client/
├── public/              # 정적 파일
├── src/
│   ├── app/            # Next.js App Router
│   │   ├── globals.css # 전역 스타일
│   │   ├── layout.tsx  # 루트 레이아웃
│   │   └── page.tsx    # 홈 페이지
│   └── shared/
│       └── assets/
│           └── fonts/  # 폰트 파일
├── next.config.ts      # Next.js 설정
├── tsconfig.json       # TypeScript 설정
└── package.json        # 프로젝트 의존성
```
