# 접근성

## 기본

- 모든 input과 textarea에 label을 연결한다.
- placeholder만으로 label을 대체하지 않는다.
- 페이지마다 h1을 하나 둔다.
- heading 순서를 지킨다.
- 텍스트와 배경 대비를 확보한다.

## 상호작용

- 아이콘 버튼에는 접근 가능한 이름을 둔다.
- 모달은 focus trap을 지원한다.
- 모달은 ESC로 닫을 수 있다.
- 페이지네이션 현재 페이지에 `aria-current="page"`를 둔다.
- toast에는 `aria-live`를 적용한다.

## 상태

- 로딩은 spinner와 텍스트 또는 sr-only 문구를 함께 둔다.
- 에러는 원인과 다음 행동을 보여준다.
- 빈 상태는 무엇이 없는지 명확히 말한다.
