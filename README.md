# 로켓 매드 토들러 — 종합 MICE 대행사 홈페이지

GitHub Pages로 배포되는 정적 원페이지 사이트입니다.

**주소**: https://anthroposphillia-ai.github.io/rocket-mad-toddler/

## 파일 구성

| 파일 | 설명 |
|---|---|
| `index.html` | 전체 페이지 (Hero / About / Services / Process / Work / Contact) |
| `style.css` | 디자인 전체 (색·폰트·레이아웃) |
| `favicon.svg` | 브라우저 탭 아이콘 |

## 수정 방법

- **색상**: `style.css` 맨 위 `:root` 의 `--accent`(포인트색), `--navy`(다크 배경), `--ink`(글자) 수정
- **회사명**: `index.html` 의 `로켓 매드 토들러` / `Rocket Mad Toddler` 전체 교체
- **숫자·실적**: `#about`·`.stats`·`#work` 안의 수치 교체 (아래는 전부 예시값)
- **서비스**: `.svc` 카드 4개 수정·추가
- **연락처**: `.crow` 의 이메일·전화·주소 교체

## 배포

`main` 브랜치에 push하면 GitHub Pages가 자동으로 갱신됩니다 (1~2분).
