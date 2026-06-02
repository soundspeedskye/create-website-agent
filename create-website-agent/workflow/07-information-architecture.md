# Preset 정보구조 설계

## 목적

route map, data model, feature use case를 도메인 중립 preset으로 확정한다.

## 실행

- root route와 주요 navigation route family를 정한다.
- 주 리소스 route family를 1개 이상 둔다.
- 보조 리소스 route와 지원 요청 route를 각각 1개 이상 둔다.
- preset account slug route와 preset management slug route를 분리한다.
- route label, slug, page slice 이름을 같은 map에서 파생한다.
- route family와 entity별 icon key를 lucide 이름으로 정한다.
- data model 목록과 entity slice 이름을 함께 정한다.
- feature use case 목록과 feature slice 이름을 함께 정한다.
- 입력이 없으면 중립 placeholder label과 slug를 사용한다.

## 참조 규칙

- `rules/02-minimum-complete-scope.md`
- `rules/09-navigation-structure.md`
- `rules/26-routing-page-map.md`
- `rules/04-fsd-structure.md`

## 완료 기준

- route family와 page slice 이름이 대응된다.
- route family와 entity icon key가 lucide-react에서 사용 가능하다.
- data model과 entity slice 이름이 대응된다.
- feature use case와 feature slice 이름이 대응된다.
