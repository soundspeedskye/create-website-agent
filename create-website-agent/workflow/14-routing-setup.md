# 라우팅 구성

## 목적

preset route map의 모든 기본 화면 경로를 만든다.

## 실행

- root route를 만든다.
- preset account slug route를 만든다.
- 주 리소스 목록, 작성, 상세, 수정 route를 만든다.
- 보조 리소스 route를 만든다.
- 지원 요청 route를 만든다.
- preset management slug route를 만든다.
- 404 fallback을 만든다.
- 라우트 컴포넌트는 각 page slice의 public API에서 가져온다.
- `../pages/pages`에서 모든 page를 한 번에 import하지 않는다.

## 참조 규칙

- `rules/26-routing-page-map.md`

## 완료 기준

- route map의 모든 기본 경로가 이동 가능하다.
- preset account slug 경로가 이동 가능하다.
- page slice public API에서 route component를 가져온다.
