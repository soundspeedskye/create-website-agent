# 보조 리소스와 지원 요청 구성

## 목적

preset의 보조 리소스와 지원 요청 흐름을 완성한다.

## 실행

- 지원 요청 route의 form을 만든다.
- 이름, 이메일, 요청 내용을 검증한다.
- 제출 결과는 toast로 알린다.
- 실제 메일 전송은 하지 않는다.
- 보조 리소스 목록 또는 상세 화면을 만든다.
- admin만 보조 리소스를 작성, 수정, 삭제할 수 있게 한다.
- root에 보조 리소스 미리보기를 연결한다.

## 참조 규칙

- `rules/34-secondary-support-flow.md`
- `rules/30-form-validation.md`
- `rules/08-toast-feedback.md`
- `rules/36-danger-actions.md`

## 완료 기준

- 지원 요청과 보조 리소스 흐름이 route map에서 동작한다.
