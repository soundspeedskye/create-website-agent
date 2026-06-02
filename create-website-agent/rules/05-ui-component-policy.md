# UI 컴포넌트 정책

## 기본

- UI kit를 강제하지 않는다.
- 기본은 Tailwind 기반 custom component다.
- shadcn, MUI, Ant Design, Chakra를 기본 설치하지 않는다.
- 반복되는 긴 class 조합은 컴포넌트로 분리한다.
- 같은 UI 패턴이 2회 이상 반복되면 추출을 검토한다.

## shared UI

- Button
- Input
- Textarea
- Modal
- Badge
- Card
- Pagination
- Tabs
- EmptyState
- ErrorState
- LoadingSpinner

## Props 기준

- `variant`
- `size`
- `disabled`
- `loading`
- `aria-label`

## 허용

- 사용자가 명시적으로 요청한 경우 UI kit를 사용할 수 있다.
- 접근성 구현이 복잡한 경우 headless 계열 사용을 검토할 수 있다.

## 금지

- 색상 hex를 컴포넌트에 직접 반복하지 않는다.
- 도메인 의미가 있는 UI를 `shared/ui`에 두지 않는다.
- 무거운 UI kit를 기본 도입하지 않는다.
