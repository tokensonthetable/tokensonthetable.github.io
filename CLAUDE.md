# CLAUDE.md — TOTT

**Tokens on the Table** — Peter Brinson's informal AI series at USC (Mondays at noon). This repo is the **public** site: `tokensonthetable/tokensonthetable.github.io` → `https://tokensonthetable.github.io/`.

- `content/` — the published markdown. `index.md` is the hub: **Meetings** and **Topics**, ordered by Peter, not by date (dates sit inline; it must not read like a blog feed). `Meetings/` = one page per meeting; `Topics/` = concepts the meetings cover, kept afterward (first: Queryable Knowledge Bases, moved from `peterbrinson.github.io/teach/AI/` 2026-10-04).
- `site/` — Quartz v4, copied from PBOH's `site/` on 2026-10-04 (same dark-only look). Built by GitHub Actions on push (`.github/workflows/deploy.yml`, `npx quartz build -d ../content`).

- `notes/` — **not part of this repo.** It is its own **private** repo (`tokensonthetable/notes`), ignored here via `.gitignore`. Holds everything that used to be the vault's `teach/AI/` (moved 2026-10-04): the TOTT brief, This Not That, the retreat deck source (still built by the vault's `build-all.ps1`), the AGP recommendation. None of it is a webpage.

**Everything else in this repo is public on GitHub**, including any file marked `publish: false` — that flag only keeps a page off the built site. Private material goes in `notes/`.

Links to PBOH or the teach site must be full URLs (separate sites); wikilinks work only between pages inside `content/`. Inside a wikilink use the page name, never a path.

Lives inside Peter's Obsidian vault as a nested repo (gitignored by the vault, like `PBOH/`), so searches run from the vault root skip it — search `TOTT/` directly.
