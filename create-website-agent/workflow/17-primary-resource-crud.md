# 주 리소스 CRUD 생성

## 목적

preset의 주 리소스 기본 기능을 완성한다.

## 실행

- 주 리소스 목록, 상세, 작성, 수정, 삭제를 만든다.
- `<child-entity>`와 optional `<nested-child-entity>`를 만든다.
- 첨부파일 메타데이터와 썸네일을 연결한다.
- user와 admin 권한을 반영한다.
- CRUD 성공과 실패를 toast로 알린다.

## 참조 규칙

- `rules/28-primary-resource-crud.md`
- `rules/36-danger-actions.md`

## 완료 기준

- 주 리소스와 `<child-entity>` CRUD가 localStorage에 반영된다.
