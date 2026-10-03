# 로켓 매드 토들러 — 종합 MICE 대행사 홈페이지

**주소**: https://anthroposphillia-ai.github.io/rocket-mad-toddler/

## 디자인 컨셉: 면 분할 큐비즘 (Facet Cubism)

"요즘 AI가 만든 사이트는 다 비슷하다"는 문제를 깨기 위해 입체파 원리를 적용했습니다.

| 입체파 원리 | 웹 구현 |
|---|---|
| 다시점 (여러 각도 동시에) | 제목 줄을 서로 다른 각도로 미세 회전 (`.h-frag`, `.tilt-l`/`.tilt-r`) |
| 면 분할 (facet) | 섹션 경계를 사선으로 자름 (`clip-path` — `.hero`, `.contact-band`, `.sec.tinted`) |
| 윤곽 이탈 (dislocated contour) | 도형과 테두리를 9px씩 어긋나게 띄움 (`.svc::after`, `.case::after`) |
| 콜라주 | 종이 그레인(노이즈 SVG) + 조각난 색면 (`.frags`) |
| 절제 팔레트 | 오커·슬레이트·차콜·종이 (일렉트릭 블루 전면 제거) |

**피한 것 (AI 티나는 요소)**: 중앙정렬 히어로, 균일한 둥근 카드, 파란 그라데이션, 반듯한 그리드 리듬, 알약 모양 버튼.

## 파일 구성

| 파일 | 설명 |
|---|---|
| `index.html` | 전체 페이지 (Hero / About / Services / Process / Work / Contact) |
| `style.css` | 디자인 전체 — 맨 위 `:root` 변수로 색 조정 |
| `favicon.svg` | 탭 아이콘 |

## 수정 방법

- **색상**: `style.css` `:root` 의 `--ochre` `--slate` `--rust` `--paper` `--dark` 수정
- **큐비즘 강도 낮추기**: `.svc::after`, `.case::after` 의 `transform: translate(...)` 값을 `0`으로
- **사선 제거**: `.hero` / `.contact-band` / `.sec.tinted` 의 `clip-path` 줄 삭제
- **기울기 제거**: `.h-frag span`, `.tilt-l`, `.tilt-r` 의 `transform` 삭제
- **회사명·실적·연락처**: `index.html` 에서 해당 텍스트 교체 (현재 전부 예시값)

## 배포

`main` 브랜치에 push하면 GitHub Pages가 자동 갱신됩니다 (1~2분).
