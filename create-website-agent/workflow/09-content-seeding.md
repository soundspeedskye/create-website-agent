# 도메인 없는 기본 콘텐츠 생성

## 목적

빈 껍데기처럼 보이지 않는 중립 콘텐츠를 만든다.

## 실행

- 실제 업종이나 브랜드를 임의 생성하지 않는다.
- 사이트명, 주 리소스명, 운영팀 같은 placeholder를 사용한다.
- 주 리소스 seed 10개 내외를 만든다.
- 보조 리소스 seed 4개 내외를 만든다.
- `<child-entity>` seed 8개 내외를 만든다.
- 필요한 경우 optional `<nested-child-entity>` seed를 만든다.
- 파일 메타데이터와 썸네일 샘플을 일부 연결한다.
- seed label은 preset label에서 파생한다.

## 참조 규칙

- `rules/27-content-preset.md`

## 완료 기준

- 도메인 없는 상태에서도 화면이 자연스럽다.
