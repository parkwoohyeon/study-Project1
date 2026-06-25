# Branch Plan

## 기본 흐름

1. `main`에서 `develop`을 만듭니다.
2. 기능 작업은 `develop`에서 `codex/feature/...` 브랜치를 나눕니다.
3. 기능 브랜치에서 작업 후 `develop`으로 pull request를 보냅니다.
4. 배포 가능한 시점에 `develop`에서 `main`으로 pull request를 보냅니다.

## 권장 issue 단위

| Branch | Issue title | 담당 영역 |
| --- | --- | --- |
| `codex/feature/project-setup` | 프로젝트 초기 세팅 | Next.js, TypeScript, lint, format |
| `codex/feature/auth` | 인증 기능 구현 | 로그인, 회원가입, 세션, 권한 |
| `codex/feature/study-posts` | 모집글 CRUD 구현 | 목록, 상세, 작성, 수정, 삭제 |
| `codex/feature/comments` | 댓글 기능 구현 | 댓글 CRUD, 권한 검사 |
| `codex/feature/applications` | 스터디 신청 기능 구현 | 신청, 승인, 거절, 마감 |
| `codex/feature/mypage` | 마이페이지 구현 | 내 글, 신청 내역, 프로필 |
| `codex/feature/search-filter` | 검색과 필터 구현 | 카테고리, 키워드, 정렬, 페이지네이션 |
| `codex/feature/deploy-ci` | 배포와 CI 구성 | Vercel, env, GitHub Actions |

## PR 체크리스트

- 기능이 요구사항대로 동작하는가?
- 권한 검사가 필요한 API와 UI에 적용되었는가?
- 빈 상태, 로딩, 에러 상태가 처리되었는가?
- DB schema 변경이 문서화되었는가?
- README 또는 관련 문서가 업데이트되었는가?
