# Toast 피드백 구성

## 목적

사용자 액션 결과를 명확하게 보여준다.

## 실행

- ToastProvider를 만든다.
- toast queue를 만든다.
- success, error, warning, info 타입을 만든다.
- 위치는 화면 가운데 하단으로 고정한다.
- 3~4초 후 자동으로 사라지게 한다.
- 닫기 버튼과 `aria-live`를 제공한다.

## 참조 규칙

- `rules/08-toast-feedback.md`

## 완료 기준

- ToastProvider와 toast queue가 준비되어 있다.
- 후속 기능에서 호출할 toast 공개 API가 제공된다.
