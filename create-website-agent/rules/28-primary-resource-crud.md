# 주 리소스 CRUD

## 기능

- 주 리소스 목록
- 주 리소스 상세
- 주 리소스 작성
- 주 리소스 수정
- 주 리소스 삭제
- `<child-entity>` 생성
- optional `<nested-child-entity>` 생성
- 첨부파일 메타데이터
- 대표 썸네일

## 관계 모델

- `<child-entity>` 이름은 preset data model에서 파생한다.
- 중첩 관계가 필요할 때만 `<nested-child-entity>`를 둔다.
- 관계형 entity는 parentId, ownerId, authorId 중 필요한 키를 가진다.

## 권한

- guest는 읽기만 가능하다.
- user는 항목과 관계형 entity를 작성할 수 있다.
- user는 본인 데이터만 수정 또는 삭제할 수 있다.
- admin은 전체 데이터를 관리할 수 있다.

## 저장

- 모든 CRUD 결과는 localStorage store에 반영한다.
- 성공과 실패는 toast로 알린다.
