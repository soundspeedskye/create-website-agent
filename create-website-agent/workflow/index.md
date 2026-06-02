# Workflow Index

## 실행 원칙

- 이 파일로 전체 순서를 먼저 확인한다.
- 단순한 단계는 개별 workflow를 열지 않고 이 요약으로 진행한다.
- 세부 기준이 필요할 때만 개별 workflow와 참조 rules를 읽는다.
- 8~12번 데이터/인증 workflow, Features, Quality 단계는 개별 workflow와 참조 rules를 확인한다.
- workflow의 참조 규칙은 그 단계에서 직접 판단 기준이 필요한 canonical rules만 둔다.
- 이미 읽은 rules는 cache를 우선 사용한다.
- 모호함, 실패, 충돌 같은 필요 사유가 있을 때만 다시 확인한다.

## Setup

1. `01-project-setup.md`: React, TS, Vite, Tailwind, npm 설정
2. `02-fsd-scaffold.md`: FSD root layer와 shared 기반 구조 생성
3. `03-theme-setup.md`: 기본 토큰과 CSS variables 설정
4. `04-icon-setup.md`: lucide-react 적용
5. `05-shared-ui-components.md`: Tailwind custom component 생성
6. `06-toast-feedback-setup.md`: 화면 가운데 하단 toast 구성

## Preset And Data

7. `07-information-architecture.md`: preset route, data model, feature 파생
8. `08-demo-data-setup.md`: entity slice와 localStorage store 계약 구성
9. `09-content-seeding.md`: 도메인 없는 seed 콘텐츠 생성
10. `10-seed-ownership-setup.md`: user 소유권 seed
11. `11-form-validation-setup.md`: feature schema 검증
12. `12-demo-auth-setup.md`: 가입, 로그인, mock 계정 인증

## Structure

13. `13-page-generation.md`: route family 기반 page 생성
14. `14-routing-setup.md`: route map 구성
15. `15-route-guard-setup.md`: 권한별 접근 제어
16. `16-ui-preset-application.md`: 도메인 중립형 UI 적용

## Features

17. `17-primary-resource-crud.md`: 주 리소스 CRUD
18. `18-resource-query-setup.md`: 검색, 필터, 페이지네이션
19. `19-upload-ux-setup.md`: 파일과 이미지 업로드 데모
20. `20-secondary-support-flow-setup.md`: 보조 리소스와 지원 요청
21. `21-management-screen-setup.md`: 관리 화면

## Quality

22. `22-accessibility-check.md`: 접근성 점검
23. `23-seo-meta-setup.md`: SEO와 메타
24. `24-theme-regeneration.md`: 컬러 변경 대응
25. `25-error-recovery-setup.md`: 저장소 복구
26. `26-final-verification.md`: 검증 명령과 완료 기준
27. `27-browser-visual-check.md`: 브라우저 시각 검수
28. `28-readme-generation.md`: README 생성
29. `29-output-summary.md`: 최종 요약
