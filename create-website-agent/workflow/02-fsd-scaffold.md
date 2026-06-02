# FSD 폴더 구조 생성

## 목적

앱의 root layer와 공통 기반을 먼저 만든다.

## 실행

- `src/app`을 만든다.
- `src/pages`를 만든다.
- `src/widgets`를 만든다.
- `src/features`를 만든다.
- `src/entities`를 만든다.
- `src/shared`를 만든다.
- `src/shared/ui`를 만든다.
- `src/shared/lib/storage`를 만든다.
- `src/shared/lib/validation`을 만든다.
- `src/shared/lib/search`를 만든다.
- `src/shared/config/theme`를 만든다.

## slice 생성 시점

- route family별 page slice는 route map 확정 후 만든다.
- feature slice는 feature use case 확정 후 만든다.
- entity slice는 data model 확정 후 만든다.
- scaffold 단계에서 특정 도메인 폴더를 하드코딩하지 않는다.

## 참조 규칙

- `rules/04-fsd-structure.md`

## 완료 기준

- FSD root layer가 준비되어 있다.
- 공통 storage, validation, search, theme 폴더가 준비되어 있다.
- 특정 도메인 이름의 slice를 임의로 만들지 않았다.
