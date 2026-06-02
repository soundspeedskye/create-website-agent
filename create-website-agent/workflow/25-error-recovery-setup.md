# 오류 복구 구성

## 목적

깨진 브라우저 저장소 때문에 앱이 멈추지 않게 한다.

## 실행

- store key가 없으면 seed를 만든다.
- JSON 파싱이 실패하면 seed로 복구한다.
- schemaVersion이 다르면 seed로 복구한다.
- users key가 없으면 빈 users store를 만든다.
- session key가 깨지면 세션만 제거한다.
- 복구 결과는 toast로 알린다.

## 참조 규칙

- `rules/25-error-recovery.md`

## 완료 기준

- 깨진 저장소에서도 앱이 빈 화면이 되지 않는다.
