# 테마와 디자인 토큰

## 위치

```txt
src/shared/config/theme/
  default-tokens.ts
  tokens.ts
  generateThemeTokens.ts
  types.ts
src/shared/lib/theme/
  applyThemeTokens.ts
```

## 기본 토큰

- 기본 primary는 `#1F4F8F`다.
- 최초 생성 중에는 컬러를 묻지 않는다.
- 기본 블루 계열 토큰으로 먼저 완성한다.
- Tailwind theme는 CSS variables와 연결한다.

## 재생성

- 사용자가 HEX를 주면 primary로 사용한다.
- 사용자가 색상 계열을 주면 안전한 primary를 선택한다.
- 대비가 부족하면 접근성 기준에 맞게 보정한다.
- 토큰 재생성은 콘텐츠와 localStorage 구조를 바꾸지 않는다.

## 규칙

- 컴포넌트에 색상 값을 하드코딩하지 않는다.
- 버튼, 링크, 활성 메뉴, focus ring은 토큰을 사용한다.
- 컬러 변경은 UI 토큰에만 영향을 준다.
