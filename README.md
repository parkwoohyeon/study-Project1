# Study Platform

스터디 모집과 운영을 연습용으로 구현하는 풀스택 협업 프로젝트입니다.

## 목표

- 프론트엔드, 백엔드, 데이터베이스, 배포 흐름을 한 프로젝트 안에서 익힙니다.
- GitHub issue, branch, pull request, code review 기반 협업 방식을 연습합니다.
- 게시판을 기본으로 하되 인증, 신청, 권한, 마이페이지까지 확장합니다.

## 추천 기술 스택

- Frontend: Next.js, React, TypeScript
- Backend: Next.js Route Handlers 또는 Server Actions
- Database: PostgreSQL
- ORM: Prisma 또는 Drizzle
- Auth: Auth.js, Supabase Auth, Clerk 중 선택
- Deploy: Vercel, Supabase 또는 Neon

## MVP

- 회원가입/로그인
- 스터디 모집글 CRUD
- 댓글
- 스터디 신청하기
- 마이페이지
- 검색/필터
- 배포

## 협업 규칙

- `main`: 배포 가능한 안정 브랜치
- `develop`: 기능 통합 브랜치
- `frontend/*`: 화면, UI 상태, 사용자 입력 처리
- `backend/*`: API, 인증, 권한, 서버 로직
- `database/*`: DB schema, 관계 설계, seed, migration
- `infra/*`: 배포, CI, 환경변수, 운영 준비
- `docs/*`: 기획, API 명세, ERD, 협업 문서
- 모든 기능은 issue 생성 후 브랜치를 만들고 PR로 병합합니다.
- PR은 최소 1명 이상 리뷰 후 병합합니다.

## 학습 브랜치

- `docs/planning`: 요구사항, 화면 흐름, 역할 분담, issue 템플릿
- `frontend/project-setup`: Next.js, TypeScript, lint, format, 폴더 구조
- `frontend/layout-navigation`: 공통 레이아웃, 헤더, 네비게이션, 반응형 UI
- `frontend/auth-pages`: 로그인, 회원가입, 인증 상태별 UI
- `frontend/board-pages`: 모집글 목록, 상세, 작성, 수정 화면
- `frontend/comment-ui`: 댓글 입력, 수정, 삭제 UI
- `frontend/mypage-ui`: 마이페이지, 내 글, 신청 내역 화면
- `backend/api-foundation`: API 구조, validation, error response 규칙
- `backend/auth-api`: 회원가입, 로그인, 세션, 권한 검사
- `backend/board-api`: 모집글 CRUD API
- `backend/comment-api`: 댓글 CRUD API
- `backend/application-api`: 스터디 신청, 승인, 거절, 마감 API
- `database/schema-design`: ERD, users, studies, comments, applications 관계 설계
- `database/migrations-seed`: migration, seed data, 개발용 샘플 데이터
- `database/query-practice`: pagination, search, filter, relation query 연습
- `infra/deploy-ci`: Vercel 배포, 환경변수, GitHub Actions
