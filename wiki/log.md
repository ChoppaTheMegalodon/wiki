# Chop Wiki — Log

> Chronological record of wiki operations. Append-only.

## [2026-04-21] init | Chop knowledge base initialized
- Created `Chop/` with `wiki/`, `raw/`, `drafts/` subdirectories
- Initialized `CLAUDE.md`, `wiki/index.md`, `wiki/log.md`
- Scope: Chop personal thesis + portfolio backbone + public wiki source. Separate from Pyth Community (ops) and Kampfire Digital (consulting).
- Trigger: decision to stand up a public Chop site with wiki + blog + video components. `BRAND_SEPARATION.md` had this as a Q1/Q2 TODO since 2026-02-06; now forcing the function.

## [2026-04-21] ingest | Stop Being Invisible — Gearside (YouTube)
- Source: https://www.youtube.com/watch?v=UlTGbJpO-fo (Charlie + Jonno, Gearside, 2026-04-09, 12:10)
- Raw: `raw/src-stop-being-invisible.md`
- Created: `wiki/src-stop-being-invisible.md`, `wiki/invisibility-tax.md`, `wiki/portfolio-as-proof.md`
- Updated: `wiki/index.md`
- First ingest of the vault. Seeds two foundational thesis pages (`invisibility-tax`, `portfolio-as-proof`) that future sources are likely to cross-reference.

## [2026-04-21] build | Quartz scaffold + GitHub repo live
- Initialized git at `Chop/` with remote `github.com/ChoppaTheMegalodon/wiki`
- Cloned Quartz v4 template, moved framework files to repo root
- Configured `quartz.config.ts`: pageTitle "Choppa's Wiki", baseUrl "choppa.wiki", analytics null, ignorePatterns include `drafts` + `raw`
- Restructured: `writings/` moved to `wiki/writings/` so Quartz's single content directory captures everything publishable
- `.gitignore` excludes `CLAUDE.md`, `drafts/`, `raw/`, `node_modules/`, `public/`
- Build command: `npm run build` → `npx quartz build --directory wiki -o public`
- Dev command: `npm run serve` → live-preview at localhost:8080
- First successful build: 12 input files, 72 output files in 5s
- CNAME file at `wiki/CNAME` → choppa.wiki
- Updated draft cross-references (`../writings/` → `../wiki/writings/`)
- Next: push to remote, configure Cloudflare Pages build command + custom domain

## [2026-04-21] domain | choppa.wiki acquired
- Domain registered for the Chop brand
- Commits the site architecture to wiki-first: the site IS the wiki
- Unlocks Quartz as the natural stack choice (Obsidian vault → static site, wikilinks work natively, graph view, backlinks)
- Updated `CLAUDE.md` Publishing Intent section and `drafts/RELEASE_PLAN.md` Open Decisions

## [2026-04-21] migrate | Existing Chop blog corpus from kampfire-digital/Blog/
- Copied 6 existing blog posts from `kampfire-digital/Blog/` → `Chop/writings/`
- Created `writings/MANIFEST.md` with inventory, thematic map, migration next steps
- Posts migrated: Why Communities Beat VCs, Creating a Community Cult(ure), Crabs in a Bucket, Foundational Community, Pseudonymity + Digital Identity, Web3 + Runescape
- Originals left in place in `kampfire-digital/Blog/` (don't break the old v1 site HTML links yet)
- Updated `CLAUDE.md` to document `writings/` folder and folder-purpose distinctions
- Reason: these are Choppa-brand content per `BRAND_SEPARATION.md`, not Kampfire — they belong in the Chop vault. Current kampfire site has been refocused as pure Kampfire consulting.

## [2026-04-21] cross-ref | 4-piece series mapped against existing corpus
- Created `drafts/CROSS_REFERENCE.md` — maps each new draft to prior-art overlap
- Finding: 2 of 4 drafts have heavy overlaps worth reframing
  - Draft 02 (Nature of Crypto Community) → 2026 update to "Why Communities Beat VCs"
  - Draft 04 (Long Eschatology) → sequel to "Creating a Community Cult(ure)"
- Updated all 4 drafts with `Prior Art` sections linking to relevant writings

## [2026-04-21] ingest | Chop's community notebook — 4 blog ideas
- Source: 4 handwritten notebook pages photographed 2026-04-21
- Raw: `raw/src-notes-why-community-hackathon-worked.md`, `raw/src-notes-nature-of-community-crypto.md`, `raw/src-notes-3rd-places-community.md`, `raw/src-notes-long-eschatology.md`
- Created: `drafts/RELEASE_PLAN.md`, `drafts/01-hackathon-worked.md`, `drafts/02-crypto-community.md`, `drafts/03-third-places.md`, `drafts/04-eschatology.md`
- 4-week community series (Apr 28 → May 19). Concrete → abstract arc. Blog + Twitter thread + LinkedIn adaptation per piece.
- Drafts are outline-level — titles, thesis, structure, thread hooks, open questions. Author fills in prose on publish day.
- Wiki concept pages will be created from each piece *after publish*, not before, to avoid double-building.
