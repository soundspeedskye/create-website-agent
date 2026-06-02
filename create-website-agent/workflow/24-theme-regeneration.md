# 테마 재생성 대응

## 목적

사용자가 색상을 바꿔도 구조와 콘텐츠를 유지한다.

## 실행

- primary 색상 요청이 있으면 토큰만 재생성한다.
- CSS variables를 다시 적용한다.
- 컴포넌트 class 구조는 유지한다.
- 콘텐츠와 localStorage seed는 변경하지 않는다.
- 색상 대비를 다시 확인한다.

## 참조 규칙

- `rules/06-theme-tokens.md`
- `rules/16-accessibility.md`

## 완료 기준

- 색상 변경 후에도 주요 화면의 대비가 유지된다.
