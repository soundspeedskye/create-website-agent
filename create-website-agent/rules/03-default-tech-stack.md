# 기본 기술 스택

## 고정 스택

- Framework: React
- Language: TypeScript
- Build: Vite
- Package manager: npm
- Architecture: FSD
- Styling: Tailwind CSS
- Routing: React Router
- Icons: lucide-react
- Form schema: Zod
- Required scripts: lint, typecheck, build

## 저장소

- 데모 데이터는 localStorage를 사용한다.
- 로그인 상태는 sessionStorage를 사용한다.
- storage 접근은 wrapper를 통해 처리한다.

## 프로젝트 기준

- init 상태의 새 프로젝트를 만든다.
- 기존 프로젝트 감지나 병합 로직은 만들지 않는다.
- UI kit는 기본으로 설치하지 않는다.

## 금지

- 서버 프레임워크를 추가하지 않는다.
- DB 클라이언트를 추가하지 않는다.
- 무거운 UI kit를 기본 설치하지 않는다.
