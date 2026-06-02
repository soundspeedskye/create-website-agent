# FSD 구조

## Layer 책임

- `app`: routing, providers, 전역 스타일, 초기화
- `pages`: 라우트 단위 화면 조립
- `widgets`: 여러 page에서 쓰는 큰 UI 블록
- `features`: 사용자 행동과 유스케이스 단위
- `entities`: 저장되거나 공유되는 도메인 모델
- `shared`: 도메인 없는 UI, lib, config

## Slice 파생

- route family마다 `pages/<route-family>/ui`를 만든다.
- feature use case마다 `features/<feature-domain>/model|ui|lib`를 만든다.
- data model마다 `entities/<entity-domain>/model|ui|lib`를 만든다.
- slice 이름은 preset의 route map, feature list, data model에서 파생한다.
- 특정 기본 도메인명을 하드코딩해 slice를 만들지 않는다.

## 배치 기준

- 페이지는 로직을 많이 가지지 않는다.
- feature 전용 schema는 `features/<feature-domain>/model`에 둔다.
- entity 타입과 seed는 `entities/<entity-domain>/model`에 둔다.
- 공통 validation은 `shared/lib/validation`에 둔다.
- storage 접근은 `shared/lib/storage`에 둔다.
- theme config는 `shared/config/theme`에 둔다.

## 검색 관련 기준

- 검색어 정규화와 페이지 계산은 `shared/lib`에 둔다.
- route-specific query 상태는 해당 feature domain의 `model`에 둔다.
- list UI 조립은 재사용 범위가 넓으면 `widgets/<list-block>`에 둔다.

## 금지

- `shared`가 특정 entity 구조를 직접 알면 안 된다.
- 모든 page를 `src/pages/pages.tsx`에 모으지 않는다.
- 여러 entity 타입을 `entities/demo/types.ts` 한 파일에 모으지 않는다.
- page가 CRUD, validation, storage 세부 구현을 직접 많이 가지지 않는다.
