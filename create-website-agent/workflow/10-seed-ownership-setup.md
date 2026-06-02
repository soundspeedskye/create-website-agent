# Seed 소유권 구성

## 목적

user와 admin의 권한 차이를 seed data에서 확인하게 한다.

## 실행

- user 소유 주 리소스를 만든다.
- 다른 사용자 소유 주 리소스를 만든다.
- user 소유 `<child-entity>`와 타인 소유 `<child-entity>`를 섞는다.
- admin은 모든 데이터를 관리할 수 있게 한다.
- ownerId 또는 authorId와 session userId를 일관되게 맞춘다.
- seed 소유권에 사용할 stable user/admin mock account id를 예약한다.

## 참조 규칙

- `rules/23-seed-ownership.md`

## 완료 기준

- user는 본인 데이터만 수정과 삭제가 가능하다.
- 초기 seed가 store 초기화 경로에 연결되어 있다.
