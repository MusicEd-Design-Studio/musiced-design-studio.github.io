# MusicEd Design Studio

An interactive music pedagogy workspace for preservice elementary teachers. Maestro Cat supports concept exploration, classroom scenarios, lesson drafting, guided reflection, and revision. The interface is in English.

## GitHub Pages 게시 방법

1. 이 ZIP의 압축을 풉니다. ZIP 파일 자체를 GitHub에 올리는 것이 아니라 **압축을 푼 파일과 폴더**를 올립니다.
2. GitHub에서 새 저장소를 만듭니다. 권장 이름: `musiced-design-studio`. 일반적인 GitHub Free 계정에서는 공개 저장소(Public)를 사용합니다.
3. 저장소의 **Add file → Upload files**에서 이 폴더 안의 파일과 폴더를 모두 업로드합니다. `assets`와 `rhythm-lab` 폴더 구조를 유지합니다.
4. 저장소 첫 화면에 `index.html`이 바로 보여야 합니다. 상위 포장 폴더나 ZIP 파일만 보인다면 파일을 한 단계 안쪽에 잘못 올린 것입니다.
5. 변경 내용을 `main` 브랜치에 커밋합니다. PR로 올렸다면 먼저 `main`에 병합합니다.
6. **Settings → Pages → Build and deployment**로 이동합니다.
7. **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**를 선택하고 **Save**를 누릅니다.
8. 게시가 완료되면 Pages 설정에 표시되는 사이트 주소를 엽니다. 오류가 있으면 저장소의 Actions 탭에서 Pages 실행 상태를 확인합니다.

주소 형식은 `https://YOUR-USERNAME.github.io/musiced-design-studio/`입니다. 실제 주소는 GitHub Pages 설정에 표시됩니다. 저장소 이름을 달리 쓰면 마지막 경로도 달라집니다.

### 업데이트

수정된 파일을 동일한 경로에 덮어쓰고 커밋하면 됩니다. 기존 저장소의 다른 프로젝트와 섞지 않도록 이 사이트 전용 저장소를 권장합니다.

## Included files

| Path | Purpose |
| --- | --- |
| `index.html` | Main teacher workspace |
| `style.css` | Responsive layout and theme |
| `app.js` | Drafts, guided coaching, scenarios, revisions, audio demos |
| `concepts.js` | 71 curriculum concept cards |
| `assets/maestro-reference.jpeg` | Supplied Maestro Cat character reference |
| `assets/cat-*.webp` | Background-removed, sharpened Maestro Cat poses cut from the supplied references |
| `rhythm-lab/` | Original student rhythm experience, retained as a teaching example |
| `.nojekyll` | Serve the package as ordinary static files |
| `CREDITS.md` | Curriculum provenance and reference links |

## Capabilities and boundaries

- 68 K–5 concept cards based on the supplied curriculum example, plus 3 clearly labeled Grade 6 proposals.
- Child-facing definitions, teacher precision notes, misconceptions, and musical experience ideas.
- Three classroom scenarios per concept, lesson drafts, self-review evidence, revision snapshots/comparison, and Markdown export.
- The coach uses authored questions and completeness checks. It is **not generative AI** and does not semantically grade arbitrary written responses.
- No API key, account system, server, package installation, or build command is needed for this version.
- Drafts, reflection dialogue, and progress are stored in the browser. They do not sync across devices or reach an instructor dashboard.
- Existing drafts on the ChatGPT-hosted address will not automatically appear on GitHub Pages because browser storage is tied to the website origin. Export any work you want to keep before switching.
- Core files and character imagery are bundled. Google Fonts is optional; system fonts are used if the font service cannot be reached.
- Music begins only after a user presses a playback control.
- Independent teaching prototype; not an official Ball State University product or a state-endorsed curriculum.

## Local preview

You can open `index.html` directly for a quick look. For normal website behavior, serve this directory over HTTP, for example with `python3 -m http.server 8000`, then open `http://localhost:8000/`. Audio and browser storage depend on browser permissions. Verify the published site on your teaching devices before classroom use.

## GitHub documentation

- Publishing source: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Uploading files: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
