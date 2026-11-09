---
name: readme-craft
description: Write or review a README, and the rest of a public repo's front door (description, topics, social preview, badges, licence, CONTRIBUTING, community links), to the standard of the most-starred open-source projects. Built from a study of 18 top READMEs (Excalidraw, Bun, Ghostty, Tauri, Ratatui, Zed, Bevy, Immich, Supabase and others). Use when asked to write, rewrite, polish or audit a README, to "make the repo look good", to prepare a repo for going public or for a launch, or when a README reads generic, AI-written or buried.
---

# readme-craft

## Why this exists

A visitor decides in about five seconds, on the first screen, whether a repo is worth their time. The best READMEs
win that screen with three things: what it is, what it looks like in use, and how to try it. Everything else is
depth for the readers who stay. The study behind this skill (2026-10-14, `research-2026-10-14.md` next to this file)
read 18 popular READMEs against one fixed question list. These rules come from what the best of them do and what
the weakest share.

The bar for a public repo is "the whole shebang": the repo art, description, README, licence and community
channels, done thoroughly and carefully.

## The first screen (the only part most visitors read)

Without scrolling, a visitor must see, in this order:
1. **The name and a one-line pitch in plain words.** Say what it is, not how it feels. Examples: "Fast, native,
   feature-rich terminal emulator" (Ghostty); "A refreshingly simple data-driven game engine built in Rust" (Bevy);
   "High performance self-hosted photo and video management solution" (Immich). Test: can a stranger say what it
   is after five seconds?
2. **One hero object** that shows the product in use: a screenshot, a short looping clip, or a release-video
   thumbnail. Not a logo cloud and not a wall of images. For anything visual, a 6-10 s MP4 (GitHub plays it inline)
   or a WebP/GIF under 8 MB beats any number of words.
3. **A way to try it:** a download link, or one command (Tauri's `npm create tauri-app@latest`, Ratatui's
   `cargo-generate` plus Hello World). Put it above the feature story. Projects that bury install (Immich, Penpot,
   Amica) lose the curious.
4. **Three to five badges at most,** each a trust signal: licence, CI, latest release or registry, community
   (Discord), and status when the project is early. Badges are evidence, not decoration.

## The 10 patterns of the best READMEs

1. **A one-line pitch in the first screen, in plain words** (above).
2. **One hero object, not a wall.**
3. **Install or try within the first screen of text.**
4. **Badges used sparingly, with a purpose.**
5. **Features shown in the shape the claim needs.**
   - Platform comparisons: a Yes/No table (Immich).
   - A framework: five or six bold design goals (Bevy).
   - A CLI: runnable commands with inline comments (Bun).
   - Otherwise, three bold-led bullets, each with a small image if visual.
   Three strong things beat twenty weak ones.
6. **Honest scope signals.** Bevy's warning that the API changes often; Ghostty's ✅/❌ roadmap table. Saying what
   doesn't work yet makes the rest believable. An early project says plainly what works, what doesn't, and what's
   next.
7. **Specific proof.** Named users, live numbers, linked sponsors, a contributor graph, star history. Generic praise
   is worth nothing; a number with a source is worth a lot.
8. **Light and dark handled deliberately.** Use `<picture>` with `prefers-color-scheme`, or GitHub's
   `#gh-light-mode-only` / `#gh-dark-mode-only` fragments (Supabase). At minimum, a transparent logo that works on
   both.
9. **Depth below the fold.** Long integration lists, full option tables and platform notes go in `<details>`, tables,
   or linked docs, so the top stays short.
10. **A next step for each audience:**
   - users: download;
   - developers: quickstart and docs;
   - contributors: CONTRIBUTING and good first issues;
   - sponsors: one line;
   - AI agents: AGENTS.md.

## Anti-patterns (they read as generic or AI-written)

- **Superlatives with no evidence** ("world's best", "blazing fast", "powerful, elegant"). Show the benchmark, the
  demo or the screenshot instead.
- **An emoji in every heading or bullet.**
- **A feature grid of identical icons with one-word labels:** a landing-page template with no product in it.
- **Empty anchor links before every heading** (`[](#anchor)`): a sign of a generated or templated file.
- **A logo cloud without context** ("and many more"). It counts only if the brands are current and linked.
- **Install buried below a long feature story.**
- **Vague claims without a number** ("used by millions"). Give a number, a date or a link.
- **Repeating the About block** at the bottom.
- **Diagrams with no stated takeaway.** Use one only where the architecture is the selling point (airi's Mermaid
  flowchart), and say what to notice.
- **A "why" section of adjectives.**
- **Claiming unbuilt features as present.** Write "will" for plans and link the roadmap.

## Outline (adapt; drop sections that have nothing true to say)

1. Centred logo (light and dark), name, one-line pitch.
2. Three to five badges.
3. Hero media.
4. Try it: download buttons and/or one build command.
5. Status, if early: two or three honest sentences.
6. Three things it does, each with a bold lead and a small image or command.
7. Comparison table, only if true and fair; otherwise skip it.
8. Developer quickstart, about 10 lines: clone, prerequisites, run, test.
9. Roadmap with ✅/❌, five to eight items, each linked to an issue.
10. Contributing: how to help, including without code (art, docs, translation, bug reports), community link,
    sponsor line, and AGENTS.md for coding agents.
11. Acknowledgements, licence and trademarks: short.

Keep the product name in one place where you can, so a rename is cheap.

## The rest of the front door ("the whole shebang")

- **Repo description** (the About box): the same one-line pitch, under about 120 characters, plus the website link.
- **Topics:** 5-10 real search terms people use for the category (check github.com/topics/<term> for traffic).
- **Social preview image:** 1280x640, readable at thumbnail size: the logo, the name, the pitch and a glimpse of the
  product. It's what shows when the link is shared.
- **Licence:** chosen deliberately, with LICENSE files present and third-party assets' licences stated.
- **CONTRIBUTING.md:** how to report a bug, the PR policy (say so clearly if PRs aren't accepted yet), the style.
- **SECURITY.md:** how to report privately.
- **CODE_OF_CONDUCT.md** if there is a community.
- **Issue and PR templates.**
- **Releases** with notes, and a CHANGELOG if versioned.
- **Community:** a Discord, Discussions or Matrix link only once someone will answer there. An empty server reads
  worse than none.
- **Trademarks:** if the name or logo matters, state that the code licence doesn't grant them.

## Method

1. **Study the category first.** Open the topic page for the category and the top 5-10 repos in it. Read each README
   against one fixed list:
   - the pitch;
   - the hero;
   - where install sits;
   - the badges;
   - the feature form;
   - the proof;
   - light/dark handling;
   - the tone.

   A small category means the bar is low, and a well-made README stands out. Confirm any HTML trick in the raw file
   (`https://raw.githubusercontent.com/<org>/<repo>/HEAD/README.md`) before copying it.
2. **Write the pitch first,** in three variants, and test each against the five-second question with a fresh
   reader (a subagent that has never seen the project).
3. **Plan the hero media before writing prose.** It's the single most important asset. Use real footage or
   synthetic stand-ins, never private test data. Ask the owner before generating art or media that represents the
   brand.
4. **Draft the README to the outline,** then cut. Every sentence must be true today; plans say "will".
5. **Review it as a visitor would:**
   - **First-screen test:** render it on GitHub (or a local GitHub-flavoured preview) at 1280x800 and at phone
     width. The pitch, hero and try-it must be visible without scrolling.
   - **Light and dark:** check both themes.
   - **Links and commands:** every link resolves, and every command runs on a clean machine.
   - **Blind read:** a fresh reader gets 10 seconds, then says what it is, who it's for and how to try it. Then it
     lists anything that reads as generic or AI-written, checked against the anti-patterns above.
6. **Do the rest of the front door,** as listed above, before the repo goes public. Going public, posting and
   creating community servers are outward-facing actions: confirm each with the owner.

## Checklist

- [ ] Pitch: one plain line that passes the five-second test
- [ ] One hero object showing the product in use, in the first screen
- [ ] Try it (download or one command) in the first screen
- [ ] Three to five purposeful badges
- [ ] Features in the shape the claim needs; three strong rather than twenty weak
- [ ] Honest status and roadmap; nothing unbuilt claimed as present
- [ ] Specific proof (numbers with sources, named users), or none
- [ ] Light and dark checked; phone width checked
- [ ] Depth folded below the first screen
- [ ] A next step for users, developers, contributors, sponsors and agents
- [ ] No anti-patterns (superlatives, emoji clutter, icon grids, empty anchors, buried install, vague claims)
- [ ] Description, topics, social preview, licence, CONTRIBUTING, SECURITY, templates, releases done
- [ ] Every link and command verified; blind read passed
