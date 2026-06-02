# 인증·권한·라우트 보호

## 계정

- user mock 계정을 제공한다.
- admin mock 계정을 제공한다.
- user mock 이메일은 `user@example.test`다.
- admin mock 이메일은 `admin@example.test`다.
- demo 비밀번호는 `password123`이다.
- 가입한 계정은 user 권한이다.
- 선택된 계정은 `<app-slug>-demo-session`에 저장한다.

## 화면

- 가입 페이지를 제공한다.
- 로그인 페이지를 제공한다.
- guest header에는 로그인과 가입 링크를 제공한다.
- 로그인 상태에서는 식별 정보와 로그아웃 버튼을 보여준다.

## 권한

- guest는 공개 page와 공개 리소스를 읽을 수 있다.
- user는 주 리소스와 `<child-entity>`를 작성할 수 있다.
- user는 본인 데이터만 수정 또는 삭제할 수 있다.
- admin은 모든 데모 데이터를 관리할 수 있다.
- admin은 관리 화면과 데모 데이터 초기화에 접근할 수 있다.

## 보호 라우트

- 주 리소스 작성 route는 user 이상만 접근한다.
- 주 리소스 수정 route는 작성자 또는 admin만 접근한다.
- 관리 route는 admin 전용이다.
- 권한 없는 접근은 안내 화면과 toast를 제공한다.

## 실패 처리

- 로그인 실패는 필드 오류 또는 상단 오류로 보여준다.
- guest가 보호 route에 접근하면 로그인과 가입 링크를 보여준다.
