# Seed 소유권

## 목적

- user와 admin 권한 차이를 seed data로 확인한다.

## 주 리소스

- user가 소유한 항목을 포함한다.
- 다른 사용자가 소유한 항목을 포함한다.
- admin이 관리할 수 있는 전체 항목을 포함한다.

## `<child-entity>`

- user가 소유한 `<child-entity>`를 포함한다.
- 다른 사용자가 소유한 `<child-entity>`를 포함한다.
- optional `<nested-child-entity>`도 authorId를 가진다.

## 기준

- seed 소유권에 사용할 stable user/admin mock account id를 예약한다.
- auth setup은 예약한 mock account id를 재사용한다.
- user 계정의 userId와 seed ownerId 또는 authorId가 일치해야 한다.
- 본인 데이터에는 수정/삭제 버튼이 보인다.
- 타인 데이터에는 수정/삭제 버튼이 보이지 않는다.
