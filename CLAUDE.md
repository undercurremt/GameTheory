# Game Theory course site — instructions for Claude

Docsify site, published by GitHub Pages from `main`. Lessons are written by the author (in Bulgarian, with English
terms and titles); Claude only files and publishes them. Never edit lesson text unless explicitly asked.

## Publishing lessons the author sends
1. Save each attached/pasted lesson to a temp file, then run `python tools/build.py add <file> [<file> ...]`.
   It detects the lesson number from the first heading (e.g. `# 001 Origins of Game Theory`), saves it as
   `part-PP/lesson_NNN_<title_slug>.md` and regenerates navigation.
   If the number can't be detected, ask the author which lesson it is.
2. `git add -A && git commit -m "Publish lesson NNN"` and push to `main`. Report the live URL:
   https://undercurremt.github.io/GameTheory/#/part-PP/lesson_NNN_<title_slug>

## Rules
- `curriculum.yaml` is the source of truth: Game Theory Master Curriculum v1.0 — 8 parts, 101 lessons (001–101)
  with core concept, guiding question, prerequisites (P) and related lessons (X).
- Generated, never edit by hand: `_sidebar.md`, `part-*/README.md`, `book-pages.js`, progress line in `README.md`.
  Change `curriculum.yaml` and run `python tools/build.py` instead.
- UI labels on generated pages are in English (Core concept, Guiding question, Prerequisites, Related lessons).
- Math in lessons (`$$…$$`, `\[…\]`, `\(…\)`) is rendered by KaTeX via a plugin in `index.html`; single `$` is not math.
- Requires `pip install pyyaml`.
