# 폼 검증 구성

## 목적

각 feature의 입력 검증을 UI와 분리한다.

## 실행

- 각 feature use case의 `model/schema.ts`에 schema를 둔다.
- 주 리소스 form을 검증한다.
- `<child-entity>` form을 검증한다.
- 보조 리소스 form과 지원 요청 form을 검증한다.
- 가입과 로그인 form을 검증한다.
- 첫 번째 오류 필드로 focus를 이동한다.

## 참조 규칙

- `rules/30-form-validation.md`

## 완료 기준

- 검증 규칙이 page 컴포넌트 내부에 길게 섞이지 않는다.
- feature slice 이름은 preset feature use case에서 파생된다.
