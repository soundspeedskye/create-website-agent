# Rules Index

## 읽기 원칙

- 모든 rules를 한 번에 읽지 않는다.
- 개별 workflow를 연 경우, 그 workflow가 참조한 rules만 읽는다.
- 이미 읽은 rule 경로와 핵심 판단 기준은 cache한다.
- 반복 참조 rule은 먼저 cache한 핵심 기준으로 판단한다.
- 실패 분석, 충돌 해결, 세부 기준 불확실 같은 필요 사유가 있을 때만 다시 읽는다.
- 병합된 canonical 문서를 우선한다.
- 오래된 세부 문서가 보이면 canonical 문서를 기준으로 판단한다.
- 인증, 접근성, 폼 검증, 위험 액션, 최종 검증 rule은 처음 읽은 문맥을 재사용한다.

## Core

- `00-document-limits.md`: md 줄 수 제한
- `01-one-shot-generation.md`: 질문 없이 기본값으로 완성
- `02-minimum-complete-scope.md`: 최소 완성 범위
- `03-default-tech-stack.md`: React, TS, Vite, FSD, Tailwind, npm
- `04-fsd-structure.md`: FSD layer와 preset slice 책임

## UI

- `05-ui-component-policy.md`: Tailwind custom component와 UI kit 정책
- `06-theme-tokens.md`: 토큰 위치와 재생성
- `07-icon-policy.md`: lucide-react
- `08-toast-feedback.md`: 화면 가운데 하단 toast
- `12-ui-preset.md`: 도메인 중립형 프리셋
- `16-accessibility.md`: 접근성 기준

## Structure

- `09-navigation-structure.md`: route family와 내비게이션
- `13-root-layout.md`: root layout
- `14-resource-list-ui.md`: 리소스 리스트 UI
- `26-routing-page-map.md`: route map과 page slice

## Data And Access

- `18-auth-access.md`: mock 계정, 권한, route guard
- `19-auth-form-flow.md`: 가입, 로그인, 로그아웃 데모 흐름
- `22-client-data-storage.md`: localStorage store
- `23-seed-ownership.md`: seed 소유권
- `24-state-management.md`: 상태 저장 위치
- `25-error-recovery.md`: 저장소 복구

## Features

- `27-content-preset.md`: 도메인 없는 seed
- `28-primary-resource-crud.md`: 주 리소스 CRUD
- `29-search-filter-pagination.md`: 검색, 필터, 페이지네이션
- `30-form-validation.md`: Zod schema
- `31-upload-thumbnail.md`: 파일, 이미지, 썸네일
- `34-secondary-support-flow.md`: 보조 리소스와 지원 요청
- `35-management-screen.md`: 관리 기본 기능
- `36-danger-actions.md`: 확인 모달
- `37-loading-error-empty.md`: 상태 화면

## Delivery

- `38-low-spec-client.md`: 가벼운 클라이언트 제한
- `39-seo-meta.md`: SEO와 메타
- `40-final-verification.md`: 기능 검증과 명령 검증
- `41-browser-visual-check.md`: 브라우저 시각 검수
- `44-delivery-notes.md`: README와 데모 제한사항
- `46-output-summary.md`: 최종 요약
