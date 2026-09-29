# MusicEd Design Studio

An interactive music pedagogy workspace for preservice elementary teachers. Maestro Cat, an orange tabby teaching partner, guides concept exploration, classroom scenarios, lesson drafting, guided reflection, revision, and a student-facing Rhythm Lab. The interface is in English.

## GitHub Pages 게시 방법

1. ZIP의 압축을 풉니다. ZIP 파일 자체가 아니라 **`musiced-design-studio` 폴더 안의 파일과 폴더**를 올립니다.
2. GitHub에서 새 저장소를 만듭니다. 권장 이름: `musiced-design-studio`. GitHub Free 계정에서는 공개 저장소(Public)를 사용합니다.
3. 저장소의 **Add file > Upload files**에서 폴더 안의 내용을 모두 끌어다 놓습니다. `assets`와 `rhythm-lab` 폴더 구조를 그대로 유지합니다.
4. 저장소 첫 화면에 `index.html`이 바로 보여야 합니다. 상위 폴더만 보인다면 한 단계 안쪽 내용을 올려야 합니다.
5. `main` 브랜치에 커밋합니다.
6. **Settings > Pages > Build and deployment**로 이동합니다.
7. **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**를 선택하고 **Save**를 누릅니다.
8. 1~2분 뒤 Pages 설정에 표시되는 주소를 엽니다. 문제가 있으면 저장소의 Actions 탭에서 배포 상태를 확인합니다.

주소 형식은 `https://YOUR-USERNAME.github.io/musiced-design-studio/`입니다.

참고: 웹 업로드 창에서는 `.nojekyll`처럼 점으로 시작하는 파일이 보이지 않거나 빠질 수 있습니다. 이 사이트는 그 파일이 없어도 정상 동작합니다.

### 업데이트

수정한 파일을 같은 경로에 다시 올려 덮어쓰고 커밋하면 됩니다.

### 바로가기 주소

- `.../musiced-design-studio/#studio` Teaching studio
- `.../musiced-design-studio/#revisions` My revisions
- `.../musiced-design-studio/#rhythm` Rhythm Lab
- 기존 `rhythm-lab/` 주소는 자동으로 `#rhythm`으로 이동합니다.

## Included files

| Path | Purpose |
| --- | --- |
| `index.html` | Page structure |
| `style.css` | Tabby-based palette, layout, light and dark themes |
| `app.js` | Concept library, studio, coaching, revisions, audio demos, Rhythm Lab |
| `concepts.js` | 71 curriculum concept cards |
| `assets/cats/` | 11 transparent Maestro Cat poses cut from the supplied character sheets |
| `assets/maestro-reference.jpeg` | Original supplied character reference |
| `rhythm-lab/index.html` | Redirect for the old Rhythm Lab address |
| `.nojekyll` | Serve the package as ordinary static files |
| `CREDITS.md` | Curriculum provenance and reference links |

## Capabilities and boundaries

- 68 K to 5 concept cards based on the supplied curriculum example, plus 3 clearly labeled Grade 6 proposals.
- The coach uses authored questions and completeness checks. It is **not generative AI** and does not grade written responses.
- No API key, account, server, or build step is needed.
- Drafts and Rhythm Lab progress are stored in the browser. They do not sync across devices. Browser storage is tied to the site address, so export any work you want to keep before switching addresses.
- Google Fonts is optional; system fonts are used if it cannot be reached.
- Sound plays only after a user presses a playback control.
- Independent teaching prototype; not an official Ball State University product or a state-endorsed curriculum.

## Local preview

Run `python3 -m http.server 8000` in this folder, then open `http://localhost:8000/`.
