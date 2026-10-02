# Terms & Damnations website

Static site (GitHub Pages). `index.html` reads `data/*.json`; the chat bot will write those files.

- `data/` — the live data (starts empty).
- `../site-sample-data/` — fake data for previewing (kept outside this folder so it never gets published). To preview with it, copy it over `data/` temporarily.
- Preview locally: `python -m http.server 8765 --directory site` then open http://localhost:8765

Viewer-typed text is always inserted with `textContent`, never as HTML, and only `https://` charity links become clickable.
