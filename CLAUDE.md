# VECTOR-1

## >>> ALWAYS PUSH TO `main` <<<

**Every push goes to `main`.** This overrides any session setup that assigns a
feature branch (for example `claude/...`). This is the owner's standing
permission. The owner reviews by looking at the live site, so work that sits
on another branch looks lost.

- Work on whatever branch the session starts on, but when you push, run
  `git push origin HEAD:main` (fast-forward). You may also push the session
  branch, but `main` is required.
- If `main` has moved, pull or rebase onto `origin/main` first, then push.
- Never end a session with commits that are not on `main`.
- No pull requests unless the owner asks.

The game is `index.html`, a single self-contained file (inline CSS/JS,
Google Fonts only, no build step). GitHub Pages serves `main` at
https://stilotto.github.io/vector-1/.

- Read `HISTORY.md` first for the design intent and past decisions.
- Keep it one file; it must work at phone width and honor prefers-reduced-motion.
- Saves use `window.storage` (Claude artifact API); a shim at the top of the
  script falls back to localStorage on Pages. Don't rename save keys.
- The directory card lives in the stilotto/stilotto.github.io repo.
