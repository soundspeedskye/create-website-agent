# 상태 관리

## 저장 위치

- 데모 데이터: localStorage
- 가입 사용자: localStorage
- 현재 로그인 상태: sessionStorage
- 검색어, 필터, page: URL query
- 모달, 로딩, 폼 입력: component state
- 테마 토큰: code file과 CSS variables

## 파생 상태

- 필터링된 리소스 목록은 저장하지 않는다.
- `<child-entity>` 수는 저장하지 않고 계산한다.
- 페이지네이션 결과는 저장하지 않고 계산한다.

## 접근

- 컴포넌트에서 storage API를 직접 호출하지 않는다.
- `shared/lib/storage` wrapper를 사용한다.
- auth 저장 접근은 feature API나 storage wrapper를 사용한다.

## 금지

- 작은 데모 앱에 무거운 전역 상태 라이브러리를 기본 도입하지 않는다.
