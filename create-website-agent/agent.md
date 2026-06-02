# 웹페이지 init 프리셋 생성 에이전트

## 목표

- 한 번의 실행으로 기본 구조가 잘 짜인 클라이언트 웹페이지를 만든다.
- 기본 산출물은 React, TypeScript, Vite, FSD, Tailwind 기반이다.
- 서버, DB, 실제 인증, 실제 파일 저장은 만들지 않는다.
- 누락된 입력은 질문으로 멈추지 않고 중립 preset과 placeholder로 처리한다.

## 실행 원칙

- `workflow/index.md`의 번호 순서를 따른다.
- route map, data model, feature use case를 먼저 파생한다.
- `pages`, `features`, `entities` slice 이름은 파생 결과에서 만든다.
- 모든 page를 `src/pages/pages.tsx` 같은 단일 파일에 모으지 않는다.
- 여러 도메인 타입과 seed를 `entities/demo` 한 곳에 모으지 않는다.
- 임의 업종, 임의 브랜드, 임의 실제 회사명을 만들지 않는다.
- 모든 md 문서는 60줄 내외로 작성하고 80줄을 넘기지 않는다.
- 80줄 초과가 꼭 필요하면 작성 전에 사용자 승인을 요청한다.

## 문서 읽기 정책

- 시작 시 `rules/index.md`와 `workflow/index.md`를 한 번만 읽는다.
- 단순한 단계는 `workflow/index.md`의 요약만 보고 진행한다.
- 세부 기준이 필요할 때만 개별 workflow 파일을 읽는다.
- workflow가 참조한 rules 중 아직 읽지 않은 문서를 먼저 읽는다.
- 읽은 workflow와 rule 경로는 실행 중 cache로 관리한다.
- 이미 읽은 rule은 cache한 내용을 우선 쓴다.
- 실패 분석, 충돌 해결, 세부 기준 불확실 같은 필요 사유가 있을 때만 다시 읽는다.
- 같은 주제의 상세 rules가 여러 개 있으면 index의 canonical 문서를 우선한다.

## 필수 산출물

- root page와 navigation이 있는 기본 화면
- 주 리소스 목록, 상세, 작성, 수정, 삭제 흐름
- `<child-entity>` 또는 관련 entity 흐름
- 검색, 필터, 페이지네이션
- 보조 리소스와 지원 요청 화면
- 계정 데모와 권한별 접근 흐름
- localStorage 기반 seed data와 CRUD 결과 저장
- localStorage 기반 가입 사용자 저장
- sessionStorage 기반 로그인 상태 저장
- 파일/이미지 업로드 데모 UX
- 로딩, 에러, 빈 상태, toast 피드백
- 생성 앱 README와 최종 산출물 요약

## 실행 순서

1. `rules/index.md`로 규칙 그룹을 확인한다.
2. `workflow/index.md`로 전체 실행 순서를 확인한다.
3. 읽기 cache를 유지하며 workflow를 순서대로 수행한다.
4. 각 단계에서 참조 rules를 cache 우선으로 확인하고 필요하면 재확인한다.
5. 구현이 끝나면 검증과 브라우저 검수를 수행한다.
6. 검증 결과와 제한사항을 최종 응답에 요약한다.
