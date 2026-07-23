# Trunkbase 0.3.2

Trunkbase turns your documents into a clean, private, searchable knowledge base
that lives entirely on your own machine.

**[⬇ Download for Windows (64-bit)](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

- **File:** `Trunkbase-Setup-x64.exe` (~357 MB) — this release also attaches the
  same file under the version-stamped name `Trunkbase_0.3.2_x64-setup.exe`; both
  are identical bytes and share the one SHA-256 below.
- **SHA-256 (both assets):** `1974f0e7cbf6cc212a36b81c073150f9ea83a29d16b80f3cd97a2c330cfd9af4`
- **Platform:** Windows 10 / 11, 64-bit
- New here? Read the **[install guide](INSTALL.md)** (it covers the SmartScreen
  prompt you'll see, and why).

---

## New in 0.3.2

- **Now supports minimize to system tray.** When closed, Trunkbase can keep
  running in the background to continuously run the local MCP server and watch
  folders.
- **Improved performance** — significantly reduced memory and CPU usage.
- **Sharper search for AI clients.** MCP now provides reranking and metadata
  filters.

### Fixes

- Fixed taskbar icon blue plate.
- Fixed Claude Desktop local MCP connections.

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
