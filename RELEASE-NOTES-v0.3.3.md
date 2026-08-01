# Trunkbase 0.3.3

Trunkbase turns your documents into a clean, private, searchable knowledge base
that lives entirely on your own machine.

**[⬇ Download for Windows (64-bit)](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

- **File:** `Trunkbase-Setup-x64.exe` (~718 MB) — this release also attaches the
  same file under the version-stamped name `Trunkbase_0.3.3_x64-setup.exe`; both
  are identical bytes and share the one SHA-256 below.
- **SHA-256 (both assets):** `85bef4418264dbddb2d0986249966d77f0c893eaf07852a36829baeaefc3ce9d`
- **Platform:** Windows 10 / 11, 64-bit
- New here? Read the **[install guide](INSTALL.md)** (it covers the SmartScreen
  prompt you'll see, and why).

> **The download is about twice the size of 0.3.2 — on purpose.** Trunkbase now
> ships its document-analysis models inside the installer instead of fetching
> them the first time you open a PDF. See the first item below.

---

## New in 0.3.3

- **PDFs work the moment you install — this is the big one.** Trunkbase now
  bundles the models it uses to analyse page layout and tables. Before 0.3.3, a
  computer that had never run these models would quietly download about 340 MB
  in the middle of processing your first PDF, with no progress shown anywhere —
  so the first file could look like it had frozen, sometimes for a long time, and
  every file behind it sat waiting. There is now nothing to download: PDF,
  scanned-image, and table extraction work offline from the very first file.
- **Much lower memory use when idle.** After processing a few documents,
  Trunkbase could hold on to roughly 3 GB while just sitting in the background.
  The search engine now hands that memory back to Windows when it goes idle.
- **The Microsoft Store build connects to Claude Desktop reliably.** The local AI
  connection is fixed for Store installs, which use a different, more locked-down
  packaging format than the direct download.
- **Trunkbase 0.3.3 is live on the Microsoft Store.** The Store build is
  code-signed, so it installs without the SmartScreen warning you'll see on the
  direct download above.

> **One optional download remains.** The search model (used for
> search-by-meaning) is still fetched once, the first time you search. Everything
> else — decomposing documents, browsing, keyword search — works offline
> immediately.

---

## What Trunkbase does

- **Decompose almost any document into clean Markdown.** Drop in a PDF, Word
  (`.docx`), PowerPoint (`.pptx`), Excel (`.xlsx`), a web page (HTML), or an
  image, and Trunkbase extracts the content into a tidy Markdown note plus
  structured metadata — no more hunting through original files.
- **Your vault, your files.** Everything is written to a plain folder you choose,
  as portable Markdown you can open in any editor. The filesystem is the source
  of truth; the app never locks your notes away in a database.
- **Hybrid search that understands meaning.** Find anything by keyword *and* by
  meaning at once, with results that jump you straight to the right section of a
  note.
- **A knowledge graph of your notes.** Trunkbase automatically links related
  notes — citations, shared tags, similar content — and shows the web of
  connections, including an interactive 3D view on the dashboard.
- **Watched folders.** Point Trunkbase at a folder (say, your Downloads), and new
  files that land there are decomposed into your vault automatically.
- **Multiple output formats per document.** Every note is always saved as
  Markdown, and you can optionally also produce HTML, JSON, YAML, or DocTags
  versions of the same document — one record, many formats, side by side.
- **A dashboard home.** See your vault at a glance — counts, recent notes, quick
  actions, and "similar notes" jump-offs.
- **Connect your AI tools (optional).** Trunkbase can expose a local connection
  so AI assistants like Claude can search, read, and — with explicit consent —
  write to your vault, all on your machine.

---

## Privacy

Everything stays on your computer by default. **No accounts and no cloud** for
your content — your documents, notes, and searches never leave your machine. Any
feature that would use an outside service (optional AI, optional anonymous usage
stats) is opt-in and clearly marked before anything is sent.

---

## Known limitations

- **Unsigned direct-download installer.** Windows SmartScreen will warn about an
  "unknown publisher" for the `.exe` above — this is expected for an unsigned
  app. Use **More info → Run anyway**; the code-signed Microsoft Store build
  won't show this warning. (Details in [INSTALL.md](INSTALL.md).)
- **Windows only for now.** macOS support is planned for a future release.

---

## Feedback

Hit a bug or have an idea? Please
[open an issue](https://github.com/Ginamus/Trunkbase-releases/issues) with a
short note on what you did and what happened. Thank you for using Trunkbase.
