# Trunkbase

**Turn any document into a clean, searchable, private knowledge base — entirely on your own machine.**

Trunkbase is a local-first desktop app that decomposes your files — PDFs, Word
documents, PowerPoint decks, Excel sheets, web pages, and images — into clean
Markdown notes plus structured metadata, saved into a folder ("vault") that you
choose and control. It never keeps the original file: it extracts what matters
and stores it as portable, future-proof Markdown you can open in any editor. On
top of your vault, Trunkbase adds fast hybrid search (keyword **and** meaning), a
dashboard, folder organization, a knowledge graph that links related notes, and
watched folders that decompose new files automatically. Everything runs on your
computer — no accounts, no cloud, no telemetry.

---

## Download

**Windows 10 or 11 (64-bit):**

➡️ **[Download the latest installer](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

That link always points at the newest release (same bytes as the versioned
asset on the release page — see below). You can also browse
[all releases](https://github.com/Ginamus/Trunkbase-releases/releases) to pick a
specific version or read the notes.

> Each release page also carries a version-stamped copy of the same installer
> (e.g. `Trunkbase_0.3.3_x64-setup.exe`), if you'd rather download a
> specific, unambiguously-versioned file for the record.

> **macOS:** coming later. This release is Windows-only.

> **AI Support:** Claude Code, Claude Desktop & Manual MCP Hosting
---

## System requirements

| | |
|---|---|
| **Operating system** | Windows 10 or Windows 11, 64-bit (x64) |
| **Disk space** | ~2 GB (the app bundles its own document engine and document-analysis models) |
| **Internet** | Not required to decompose documents — as of 0.3.3 the document models ship inside the installer, so PDFs work offline from the first file. One optional download remains: the search-by-meaning model, fetched once the first time you search. |
| **macOS / Linux** | Not yet — macOS is planned for a later release. |

---

## Installing (first time)

1. Download the installer using the button above.
2. Double-click the downloaded **`Trunkbase-Setup-x64.exe`** (or the
   version-stamped `Trunkbase_0.3.3_x64-setup.exe`, if that's the one you
   grabbed — they're the same file).
3. **You will see a blue "Windows protected your PC" screen.** This is expected —
   see the note just below on why. Click **More info**, then **Run anyway**.
4. Follow the installer, then launch Trunkbase.
5. On first launch, pick or create a **vault** folder — this is where all your
   decomposed notes will live. You own it; it's just a normal folder on your disk.

A fuller walkthrough (with uninstall steps) is in **[INSTALL.md](INSTALL.md)**.

### Why does Windows warn me?

This public installer is **not code-signed yet**. Code signing is a paid
certificate that tells Windows who published an app; without it, Windows
SmartScreen shows the "unknown publisher" warning for *any* new app, safe or not.
A **code-signed Microsoft Store build is coming** and won't show this warning.
Until then, the **More info → Run anyway** step is how you tell Windows you trust
this download. If that trade-off isn't comfortable for you, we'd suggest waiting
for the signed build.

---

## What to expect

Trunkbase is an early product under active development. It's genuinely useful
today, but expect the occasional rough edge, and please keep a copy of anything
important elsewhere while you get comfortable with it.

- **Windows-only** for this release; **macOS** comes later.
- **The public installer is unsigned**, so you'll see the SmartScreen prompt
  above (a signed Microsoft Store build is coming).
- **Found a bug or have an idea?** Please open an
  [issue](https://github.com/Ginamus/Trunkbase-releases/issues) — a short
  description of what you did and what happened is a huge help.

---

## Your privacy

Everything stays on your machine. Trunkbase has **no accounts, no telemetry, and
no cloud** — your documents, notes, and searches never leave your computer.
Optional AI features that use an outside service are strictly opt-in and clearly
marked before anything is sent; the default is fully local and private.
