# Tailwind custom component 생성

## 목적

반복 UI를 Tailwind 기반 custom component로 분리한다.

## 실행

- Button, Input, Textarea, Modal을 만든다.
- Badge, Card, Pagination, Tabs를 만든다.
- EmptyState, ErrorState, LoadingSpinner를 만든다.
- 반복 class 조합은 variant와 size props로 관리한다.
- 도메인 의미가 없는 UI만 `shared/ui`에 둔다.

## 참조 규칙

- `rules/05-ui-component-policy.md`

## 완료 기준

- 반복되는 긴 Tailwind class가 페이지에 흩어지지 않는다.
- 주요 UI는 재사용 가능한 props를 가진다.
