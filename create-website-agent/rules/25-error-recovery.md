# 저장소 오류 복구

## 대상

- store key가 없으면 seed data를 생성한다.
- JSON 파싱이 실패하면 seed data로 복구한다.
- schemaVersion이 맞지 않으면 seed data로 복구한다.
- users key가 없으면 빈 users store를 만든다.
- session key가 깨져 있으면 세션만 제거한다.

## 사용자 안내

- 복구가 발생하면 toast로 알린다.
- 초기화 버튼은 관리 화면에 둔다.
- 초기화는 데모 데이터만 복원한다.
- 가입 사용자 저장소는 초기화하지 않는다.

## 방어

- 존재하지 않는 id 접근은 오류 화면 또는 빈 상태로 처리한다.
- 끊어진 관계 참조는 화면에서 무시한다.
- 잘못된 route parameter는 404로 보낸다.

## 금지

- 깨진 localStorage 때문에 앱 전체가 빈 화면이 되면 안 된다.
- 사용자가 만든 가입 계정을 임의 삭제하지 않는다.
