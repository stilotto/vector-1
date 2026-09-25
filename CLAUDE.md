# VECTOR-1

The game is `index.html`, a single self-contained file (inline CSS/JS,
Google Fonts only, no build step). GitHub Pages serves `main` at
https://stilotto.github.io/vector-1/.

- Read `HISTORY.md` first for the design intent and past decisions.
- Keep it one file; it must work at phone width and honor prefers-reduced-motion.
- Saves use `window.storage` (Claude artifact API); a shim at the top of the
  script falls back to localStorage on Pages. Don't rename save keys.
- The directory card lives in the stilotto/stilotto.github.io repo.
