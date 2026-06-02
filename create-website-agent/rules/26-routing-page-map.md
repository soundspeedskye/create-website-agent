# 라우팅과 페이지 맵

## 파생 규칙

- route map은 preset의 route family에서 만든다.
- page slice는 route family slug와 같은 이름을 사용한다.
- account route와 page slice는 preset account slug에서 파생한다.
- management route와 page slice는 preset management slug에서 파생한다.
- fallback route는 `pages/error`를 사용한다.

## 필수 route family

- `/`: root page
- `/<primary-resource>`: 주 리소스 목록
- `/<primary-resource>/new`: 주 리소스 작성
- `/<primary-resource>/:itemId`: 주 리소스 상세
- `/<primary-resource>/:itemId/edit`: 주 리소스 수정
- `/<support-route>`: 지원 요청 폼
- `/<secondary-resource>`: 보조 리소스 목록 또는 안내
- `/<preset-account-slug>`: account 흐름
- `/<preset-management-slug>`: 관리 대시보드

## 예외

- 존재하지 않는 경로는 404 화면을 보여준다.
- 권한 없는 경로는 안내 화면과 toast를 제공한다.
