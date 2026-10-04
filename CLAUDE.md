# CLAUDE.md — TOTT

**Tokens on the Table** — Peter Brinson's informal AI series at USC (Mondays at noon). This repo is the **public** site: `tokensonthetable/tokensonthetable.github.io` → `https://tokensonthetable.github.io/`.

- `content/` — the published markdown. `index.md` is the series page; `Meetings/` holds one page per meeting.
- `site/` — Quartz v4, copied from PBOH's `site/` on 2026-10-04 (same dark-only look). Built by GitHub Actions on push (`.github/workflows/deploy.yml`, `npx quartz build -d ../content`).

**Everything in this repo is public on GitHub**, including any file marked `publish: false` — that flag only keeps a page off the built site. Private planning lives in the vault at `teach/AI/Tokens on the Table/`, not here.

Links to PBOH or the teach site must be full URLs (separate sites); wikilinks work only between pages inside `content/`. Inside a wikilink use the page name, never a path.

Lives inside Peter's Obsidian vault as a nested repo (gitignored by the vault, like `PBOH/`), so searches run from the vault root skip it — search `TOTT/` directly.
