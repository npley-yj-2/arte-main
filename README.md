# arte 라이브러리 스크롤 모션

Figma 시안을 기반으로 만든, 스크롤에 반응하는 정적 HTML 사이트입니다.
[GSAP](https://gsap.com)의 ScrollTrigger로 각 섹션의 등장 애니메이션을 구현했습니다.

## 구조

- `public/` — 사이트 원본 (`arte-main.html`, `arte-document.html`, `arte-location.html`, `arte-search.html`)과 각 페이지가 쓰는 이미지 에셋
- `docs/` — GitHub Pages로 배포되는 사본. `docs/index.html`과 `docs/arte-main.html`은 둘 다 `public/arte-main.html`과 항상 같은 내용으로 유지합니다 (GitHub Pages가 요구하는 `index.html`과, 다른 페이지들이 링크하는 `arte-main.html` 파일명을 동시에 만족시키기 위함).

## 로컬에서 보기

빌드 과정이 없는 순수 정적 파일이라 `public/` 디렉터리를 아무 정적 서버로 열면 됩니다.

```console
npx serve public
```

## 배포

`docs/` 아래 내용이 GitHub Pages로 그대로 서빙됩니다: https://npley-yj-2.github.io/arte-main/
