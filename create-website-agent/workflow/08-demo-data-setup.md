# localStorage 데모 데이터와 사용자 구성

## 목적

preset data model의 저장 계약과 entity slice를 먼저 만든다.

## 실행

- `<app-slug>-demo-store` key를 사용한다.
- 가입 사용자는 `<app-slug>-demo-users` key를 사용한다.
- 기존 store가 있으면 덮어쓰지 않는다.
- 기존 users가 있으면 덮어쓰지 않는다.
- data model별 `entities/<entity-domain>/model`을 만든다.
- CRUD 대상 entity는 byId/allIds 구조로 둔다.
- 관계형 entity는 parentId, ownerId, authorId 중 필요한 키를 둔다.
- store 조립과 초기화는 `entities/demo-store/model`에 둔다.
- 이후 seed 단계가 주입할 초기 data entry point를 준비한다.
- 관리 초기화가 seed를 복원할 수 있는 함수를 준비한다.

## 참조 규칙

- `rules/22-client-data-storage.md`
- `rules/24-state-management.md`

## 완료 기준

- data model에서 entity slice 이름이 파생되어 있다.
- entity slice와 store contract가 data model에서 파생되어 있다.
- seed 콘텐츠를 주입할 초기화 경로가 준비되어 있다.
- 가입 사용자와 세션 저장 key가 준비되어 있다.
