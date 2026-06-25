# Branch Plan

## 기본 흐름

1. `main`에서 `develop`을 만듭니다.
2. 작업은 `develop`에서 카테고리별 브랜치를 나눕니다.
3. 작업 브랜치에서 구현 후 `develop`으로 pull request를 보냅니다.
4. 배포 가능한 시점에 `develop`에서 `main`으로 pull request를 보냅니다.

## 브랜치 카테고리

| Prefix | 목적 | 공부 포인트 |
| --- | --- | --- |
| `docs/*` | 기획과 협업 문서 | 요구사항, ERD, API 명세, issue 분리 |
| `frontend/*` | 사용자 화면 | React component, state, form, routing, responsive UI |
| `backend/*` | 서버 기능 | API 설계, 인증, 권한, validation, error handling |
| `database/*` | 데이터 설계 | PostgreSQL, ORM, relation, migration, query |
| `infra/*` | 배포와 운영 | Vercel, env, CI, production checklist |

## 권장 issue 단위

| Branch | Issue title | 담당 영역 |
| --- | --- | --- |
| `docs/planning` | 프로젝트 기획 정리 | 요구사항, MVP, 역할 분담, 화면 흐름 |
| `frontend/project-setup` | 프론트 초기 세팅 | Next.js, TypeScript, lint, format, 폴더 구조 |
| `frontend/layout-navigation` | 공통 레이아웃 구현 | header, navigation, responsive layout |
| `frontend/auth-pages` | 인증 화면 구현 | login, signup, session UI, form handling |
| `frontend/board-pages` | 게시판 화면 구현 | list, detail, create, edit, delete UI |
| `frontend/comment-ui` | 댓글 UI 구현 | comment form, edit mode, delete confirm |
| `frontend/application-ui` | 스터디 신청 화면 구현 | apply button, applicant list, approve/reject UI |
| `frontend/mypage-ui` | 마이페이지 UI 구현 | profile, my posts, my applications |
| `frontend/search-filter-ui` | 검색과 필터 화면 구현 | keyword search, category filter, sorting, pagination UI |
| `backend/api-foundation` | API 기본 구조 구현 | route structure, validation, error response |
| `backend/auth-api` | 인증 API 구현 | signup, login, logout, session, authorization |
| `backend/board-api` | 게시글 API 구현 | studies CRUD, ownership check |
| `backend/comment-api` | 댓글 API 구현 | comments CRUD, permission check |
| `backend/application-api` | 신청 API 구현 | apply, approve, reject, close recruitment |
| `database/schema-design` | DB schema 설계 | users, studies, comments, applications, relations |
| `database/migrations-seed` | migration과 seed 구성 | migration workflow, sample data |
| `database/query-practice` | 조회 쿼리 연습 | pagination, search, category filter, sorting |
| `infra/deploy-ci` | 배포와 CI 구성 | Vercel, env, GitHub Actions |

## PR 체크리스트

- 기능이 요구사항대로 동작하는가?
- 권한 검사가 필요한 API와 UI에 적용되었는가?
- 빈 상태, 로딩, 에러 상태가 처리되었는가?
- DB schema 변경이 문서화되었는가?
- README 또는 관련 문서가 업데이트되었는가?
