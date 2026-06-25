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
- `codex/feature/*`: 기능별 작업 브랜치
- 모든 기능은 issue 생성 후 브랜치를 만들고 PR로 병합합니다.
- PR은 최소 1명 이상 리뷰 후 병합합니다.

## 기능 브랜치

- `codex/feature/project-setup`: Next.js 초기 세팅, 린트, 포맷, 폴더 구조
- `codex/feature/auth`: 로그인, 회원가입, 세션, 권한 처리
- `codex/feature/study-posts`: 스터디 모집글 목록, 상세, 작성, 수정, 삭제
- `codex/feature/comments`: 댓글 작성, 수정, 삭제
- `codex/feature/applications`: 스터디 신청, 승인, 거절, 모집 상태
- `codex/feature/mypage`: 내 스터디, 신청 내역, 프로필
- `codex/feature/search-filter`: 검색, 카테고리, 정렬, 페이지네이션
- `codex/feature/deploy-ci`: 배포, 환경변수 문서화, 기본 CI
