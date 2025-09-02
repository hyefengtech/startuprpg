# SideFund · 1인 VC 포트폴리오 (GitHub Pages)

## 1) 사용법
1. 이 폴더 전체를 GitHub에 새 레포로 업로드 (예: `yourname/sidefund`).
2. 레포 → Settings → Pages → Branch: `main` (또는 `master`) / root 선택 → Save.
3. 30초 내 배포된 URL로 접근 (`https://yourname.github.io/sidefund`).

## 2) 수정 포인트
- `_data/portfolio.yml`에 당신의 실제 서비스들을 추가/수정.
- `index.md` 히어로 문구/CTA 수정.
- `about.md` 소개/투자 논문(Thesis) 서술.
- 블로그는 `_posts` 폴더에 마크다운 추가 (`YYYY-MM-DD-title.md`).

## 3) 팁
- 프로젝트별 '케이스 스터디'가 있으면 `case_url`에 링크.
- 썸네일/로고가 필요하면 `/assets`에 저장 후 카드에 이미지 태그를 추가하세요.
- 도메인 연결은 Settings → Pages → Custom domain.

## 4) 로컬 미리보기(선택)
- Ruby/Jekyll 환경에서 `bundle exec jekyll serve`로 미리보기 가능.
- 단, GitHub Pages는 이 레포 그대로도 빌드됩니다(테마 없음, 커스텀 레이아웃).