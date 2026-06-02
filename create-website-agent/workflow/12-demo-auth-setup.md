# 가입·로그인과 데모 인증

## 목적

서버 없이 가입, 로그인, 권한 흐름을 테스트할 수 있게 한다.

## 실행

- user mock 계정을 만든다.
- admin mock 계정을 만든다.
- mock 계정 이메일은 `user@example.test`, `admin@example.test`를 사용한다.
- mock account id는 seed 소유권 단계에서 예약한 id를 재사용한다.
- 가입 form과 로그인 form을 만든다.
- 가입 사용자는 `<app-slug>-demo-users`에 저장한다.
- 로그인 세션은 `<app-slug>-demo-session`에 저장한다.
- mock 계정도 로그인할 수 있게 한다.
- logout은 세션만 제거한다.

## 참조 규칙

- `rules/18-auth-access.md`
- `rules/19-auth-form-flow.md`
- `rules/30-form-validation.md`

## 완료 기준

- guest, user, admin 상태를 화면에서 확인할 수 있다.
- 가입 후 user 상태로 로그인된다.
- 로그아웃 후 다시 로그인할 수 있다.
