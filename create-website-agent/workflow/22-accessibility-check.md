# 접근성 점검

## 목적

키보드와 보조기술 사용자가 주요 흐름을 사용할 수 있게 한다.

## 실행

- 모든 input에 명시적 label을 연결한다.
- icon-only 버튼에 aria-label을 둔다.
- 현재 route와 현재 page에 aria-current를 둔다.
- modal은 focus trap과 escape 닫기를 지원한다.
- danger modal의 취소 버튼을 기본 focus로 둔다.
- toast는 aria-live를 사용한다.
- 색상 대비를 확인한다.

## 참조 규칙

- `rules/16-accessibility.md`
- `rules/36-danger-actions.md`

## 완료 기준

- 주요 화면을 키보드로 이동하고 제출할 수 있다.
