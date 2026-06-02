# 기본 페이지 생성

## 목적

preset route family별 page를 빈 껍데기 없이 만든다.

## 실행

- root page는 `pages/<root-family>/ui`에 둔다.
- account page는 `pages/<preset-account-slug>/ui`에 둔다.
- 주 리소스 page는 `pages/<primary-resource>/ui`에 둔다.
- 보조 리소스 page는 `pages/<secondary-resource>/ui`에 둔다.
- 지원 요청 page는 `pages/<support-route>/ui`에 둔다.
- management page는 `pages/<preset-management-slug>/ui`에 둔다.
- 404와 접근 거부는 `pages/error/ui`에 둔다.
- page 내부 반복 UI는 같은 page slice의 `ui`에 둔다.

## 참조 규칙

- `rules/02-minimum-complete-scope.md`
- `rules/37-loading-error-empty.md`

## 완료 기준

- 각 route는 의미 있는 placeholder 콘텐츠를 가진다.
- page 파일은 라우트 조립 중심이며 도메인 로직을 직접 많이 가지지 않는다.
