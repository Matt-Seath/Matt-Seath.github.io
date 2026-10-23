# Larry — static site

A single-file, dependency-free landing page for Larry. Just `index.html` (plus this
README). Nothing to build; GitHub Pages serves it as-is.

It's intentionally **public-safe**: no hostnames, numbers, accounts, or infra details —
just a fun presence page. (It can't talk to the live Larry; the gateway is private.)

## Deploy to GitHub Pages

**Option A — project site** (serves at `https://<you>.github.io/<repo>/`)
1. Put `index.html` at the root of any **public** repo (or a private one if you have GitHub Pro).
2. Repo → **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)` → **Save**.
4. Live in ~1 min at `https://<you>.github.io/<repo>/`.

**Option B — user site** (serves at `https://<you>.github.io/`)
1. Use a repo named exactly `<you>.github.io`.
2. Push `index.html` to its `main` branch → Pages is automatic.

## Notes
- Plain HTML needs no `.nojekyll` and no Jekyll config.
- To change the look: it's all inline in `index.html` — colors are CSS variables in `:root`
  near the top; copy for the feature cards and the mascot one-liners are in the `<body>`/`<script>`.
- Dark/light follows the system and has a manual toggle (top-right).
