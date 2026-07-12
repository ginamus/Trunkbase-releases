# Trunkbase v0.1.0-beta.1

**The first public beta.** Trunkbase turns your documents into a clean, private,
searchable knowledge base that lives entirely on your own machine.

**[⬇ Download for Windows (64-bit)](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

- **File:** `Trunkbase-Setup-x64.exe` (~370 MB) — this release also attaches the
  same file under the version-stamped name
  `Trunkbase_0.1.0-beta.1_x64-setup.exe`; both are identical bytes and share the
  one SHA-256 below.
- **SHA-256 (both assets):** `258402ca90f47f7598e4e21b730ed25955d7b01dee8b4977a90e7170575a0f91`
- **Platform:** Windows 10 / 11, 64-bit
- New here? Read the **[install guide](INSTALL.md)** (it covers the SmartScreen
  prompt you'll see, and why).

---

## What Trunkbase does today

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
- **Connect your AI tools (optional).** Trunkbase can expose a local, read-only
  connection so AI assistants like Claude can search and read your vault — with
  your explicit per-connection consent, all on your machine.

---

## Privacy

Everything stays on your computer. **No accounts, no telemetry, no cloud.** Your
documents, notes, and searches never leave your machine. Any feature that would
use an outside service is opt-in and clearly marked before anything is sent.

---

## Known limitations

- **Unsigned installer.** Windows SmartScreen will warn about an "unknown
  publisher" — this is expected for an unsigned app. Use **More info → Run
  anyway**; code signing is planned for a later release. (Details in
  [INSTALL.md](INSTALL.md).)
- **Windows only for now.** macOS support is planned for a future release.
- **It's a beta.** Shared with a small circle of trusted testers. Expect rough
  edges, and keep your own copy of anything important while you try it out.

---

## Feedback

Hit a bug or have an idea? Please
[open an issue](https://github.com/Ginamus/Trunkbase-releases/issues) with a
short note on what you did and what happened. Thank you for testing.
