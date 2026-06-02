# create-website-agent

React + TypeScript + Vite + FSD + Tailwind 기반의 클라이언트 웹페이지 init 에이전트 문서 모음입니다.
route, feature, entity slice를 preset에서 파생하는 v3 버전입니다.

## 사용 방법

1. 이 폴더를 사용할 프로젝트로 옮긴다.
2. `agent.md`를 에이전트의 시작 지시문으로 사용한다.
3. `workflow/index.md`의 순서와 읽기 정책을 따르게 한다.
4. `rules/index.md`의 canonical/cache 정책에 따라 rules를 참조하게 한다.

## 기본 산출물

- 서버 없는 클라이언트 웹페이지
- preset 기반 route map과 navigation
- list/detail/form 중심의 주 리소스 흐름
- 보조 리소스와 지원 요청 흐름
- 계정 데모와 권한별 접근 흐름
- 도메인 slice 기반 pages, features, entities
- localStorage 데모 데이터
- sessionStorage 로그인 상태
- Tailwind 기반 custom component
- lucide-react 아이콘

## init 원칙

- 특정 업종이나 리소스 도메인을 고정하지 않는다.
- 사용자가 도메인을 주면 route, feature, entity 이름을 거기서 파생한다.
- 입력이 없으면 중립 placeholder preset으로 완성한다.

## 문서 제한

- 모든 md 파일은 60줄 내외를 목표로 한다.
- 어떤 md 파일도 80줄을 넘기지 않는다.
- 80줄 초과가 필요하면 사용자 승인을 먼저 받아야 한다.

## 제한사항

- 실제 서버 인증이 아니다.
- 비밀번호 저장은 데모 검증값이며 운영 보안 구현이 아니다.
- 실제 DB를 사용하지 않는다.
- 파일 원본을 저장하지 않는다.
- 기본 콘텐츠는 도메인 없는 placeholder만 사용한다.
