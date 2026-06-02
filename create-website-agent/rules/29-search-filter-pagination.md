# 검색·필터·페이지네이션

## 검색

- 검색 대상은 제목, 내용, 작성자 또는 소유자다.
- 검색어는 앞뒤 공백을 제거한다.
- 검색어 비교는 대소문자를 구분하지 않는다.

## 필터

- 카테고리 필터는 전체 + preset category 목록으로 둔다.
- 필터는 URL query에 반영한다.
- 필터 변경 시 1페이지로 돌아간다.

## 페이지네이션

- 페이지당 항목은 10개다.
- `q`, `category`, `page`를 URL query에 반영한다.
- 범위를 벗어난 page는 마지막 유효 page로 보정한다.

## 위치

- 검색어 정규화와 페이지 계산은 `shared/lib/search`에 둔다.
- route-specific query model은 해당 `features/<feature-domain>/model`에 둔다.
