# 클라이언트 데이터 저장

## key

- localStorage key는 `<app-slug>-demo-store`다.
- 가입 사용자 key는 `<app-slug>-demo-users`다.
- sessionStorage key는 `<app-slug>-demo-session`이다.

## store 구조

- `schemaVersion`
- `seedVersion`
- `updatedAt`
- `app`
- `routes`
- `navigation`
- `entities`
- `entityData`
- `uploads`
- `relationships`

## users 구조

- `schemaVersion`
- `updatedAt`
- `users.byId`
- `users.allIds`
- user 필드는 id, role, email, name, password, createdAt이다.

## data model 파생

- preset은 entity domain 목록을 먼저 정의한다.
- 각 entity는 id, title 또는 label, createdAt을 가진다.
- CRUD 대상 entity는 byId/allIds 구조로 저장한다.
- 관계형 항목은 sourceId, targetId 또는 parentId를 가진다.
- 도메인 seed와 타입은 각 `entities/<entity-domain>/model`에 둔다.
- store 조립은 `entities/demo-store/model`에서 담당한다.

## 규칙

- mock data는 seed로 제공한다.
- CRUD 결과는 localStorage에 저장한다.
- 가입 사용자는 localStorage에 저장한다.
- sessionStorage에는 현재 사용자 세션만 저장한다.
- 파일 원본은 저장하지 않는다.
- 이미지는 작은 썸네일만 저장한다.
