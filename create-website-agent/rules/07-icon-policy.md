# 아이콘 정책

## 기본

- `lucide-react`를 사용한다.
- 아이콘은 버튼과 상태 표시를 보조한다.
- 장식용 아이콘 남발을 피한다.

## 크기

- 일반 아이콘은 18~20px를 기본으로 한다.
- 작은 버튼은 16px를 사용할 수 있다.
- 모바일에서도 터치 영역은 44px 이상을 유지한다.

## 기본 매핑

- 검색: `Search`
- 작성 또는 추가: `Plus`
- 수정: `Pencil`
- 삭제: `Trash2`
- 업로드: `Upload`
- 파일: `FileText`
- 이미지: `Image`
- `<child-entity>`: preset metadata에서 선택
- 보조 리소스: `Megaphone`
- 지원 요청: `Mail`
- 관리: `LayoutDashboard`, `Shield`
- 로그아웃: `LogOut`

## 접근성

- 아이콘만 있는 버튼은 `aria-label`을 둔다.
- 의미 없는 장식 아이콘은 `aria-hidden`을 사용한다.
