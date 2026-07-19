# Trunkbase 0.3.1

Trunkbase turns your documents into a clean, private, searchable knowledge base
that lives entirely on your own machine.

**[⬇ Download for Windows (64-bit)](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

- **File:** `Trunkbase-Setup-x64.exe` (~357 MB) — this release also attaches the
  same file under the version-stamped name `Trunkbase_0.3.1_x64-setup.exe`; both
  are identical bytes and share the one SHA-256 below.
- **SHA-256 (both assets):** `473c1cede5b3d1350ee702fb2766826a3c24a3ba269c4aae0b2077e534f1bf53`
- **Platform:** Windows 10 / 11, 64-bit
- New here? Read the **[install guide](INSTALL.md)** (it covers the SmartScreen
  prompt you'll see, and why).

---

## New in 0.3.1

Everything since the first beta, in one release:

- **日本語 (Japanese) interface.** The whole app is now available in Japanese,
  with an English · 日本語 · System language switch that changes instantly.
- **Connect your AI tools to write, not just read.** With your explicit
  per-scope consent, AI assistants like Claude can now add tags, write folder
  descriptions, and create or update notes in vaults you mark writable — never
  delete your notes, never touch original files.
- **Tunnels.** Map an external folder into your vault as a paths-only index
  (Trunkbase reads *no* file content until you choose to), then decompose
  entries on demand — individually or in bulk.
- **Vault management.** Rename, relocate, or delete a vault from a per-row menu,
  with confirmations and a recycle-bin option — no vault content is moved on disk.
- **Opt-in, anonymous usage stats.** Off by default and asked once; anonymous
  and content-blind, with a clear on/off switch in Settings → Privacy.
- **A lighter, tidier build** and UI polish — a branded loading screen, a
  cleaned-up About section, and a choice of 3D or Simple knowledge-graph style.

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

- **Unsigned installer.** Windows SmartScreen will warn about an "unknown
  publisher" — this is expected for an unsigned app. Use **More info → Run
  anyway**; a code-signed Microsoft Store build is coming and won't show this
  warning. (Details in [INSTALL.md](INSTALL.md).)
- **Windows only for now.** macOS support is planned for a future release.

---

## Feedback

Hit a bug or have an idea? Please
[open an issue](https://github.com/Ginamus/Trunkbase-releases/issues) with a
short note on what you did and what happened. Thank you for using Trunkbase.
