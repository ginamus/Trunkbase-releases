# Installing Trunkbase on Windows

A step-by-step guide to installing, first-run setup, and uninstalling Trunkbase
on Windows 10 and 11. If you just want the short version, the
[README](README.md) has it.

---

## Before you start

- **You need:** Windows 10 or 11, 64-bit. About 2 GB of free disk space.
- **You don't need:** an account, a license key, or an internet connection to
  use the app. (A single search model downloads automatically the first time you
  search; after that Trunkbase runs fully offline. Decomposing documents needs no
  download at all — the document models ship inside the installer.)

---

## Step 1 — Download the installer

Open the download page and get the latest installer:

➡️ **[Trunkbase-Setup-x64.exe](https://github.com/Ginamus/Trunkbase-releases/releases/latest/download/Trunkbase-Setup-x64.exe)**

The file is around 718 MB — it bundles the whole document engine *and* the
document-analysis models, so there's nothing else to install and nothing to
download when you open your first PDF. Each release page also carries the exact
same bytes under a version-stamped filename (e.g. `Trunkbase_0.3.3_x64-setup.exe`),
if you'd rather download that one for the record — either file installs the
same app.

> _[Screenshot: the GitHub Releases page for Trunkbase, with the
> `Trunkbase-Setup-x64.exe` asset highlighted under the latest release's Assets
> list.]_

---

## Step 2 — Run the installer past the SmartScreen prompt

Double-click the downloaded `.exe`. Because the public installer is **not yet
code-signed** (see [Why the warning?](#why-the-warning) below), Windows will show
a blue **"Windows protected your PC"** screen.

1. Click the small **More info** link.
2. A **Run anyway** button appears at the bottom — click it.

> _[Screenshot: the blue Windows SmartScreen dialog reading "Windows protected
> your PC", with the "More info" link circled.]_

> _[Screenshot: the same dialog after clicking "More info", now showing the
> app name and an unknown-publisher line, with the "Run anyway" button
> highlighted.]_

If you don't see a **More info** link, your organization may block unsigned apps
by policy — in that case this build isn't installable on that machine, and you'll
want to wait for the signed Microsoft Store release.

---

## Step 3 — Complete the installer

Follow the prompts to finish installation, then launch Trunkbase from the Start
menu or the desktop shortcut.

> _[Screenshot: the Trunkbase setup wizard on its install-location step.]_

---

## Step 4 — First run: choose your vault

On first launch, Trunkbase asks you to **create a new vault** or **open an
existing folder** as your vault. A vault is simply a folder on your disk where
all your decomposed notes will be written — plain Markdown files you fully own
and can open in any editor.

> _[Screenshot: the Trunkbase onboarding screen with "Create vault" and "Open
> folder" buttons.]_

Once your vault is set, drag a document (PDF, Word, PowerPoint, Excel, a web
page, or an image) into the app and Trunkbase will decompose it into a clean
Markdown note. That's it — you're up and running.

---

## Why the warning? {#why-the-warning}

Windows SmartScreen shows "unknown publisher" for any application that isn't
**code-signed** — a paid certificate that vouches for the publisher's identity.
The public installer ships unsigned, so the warning appears even though the
download is the same file published on this repo's Releases page. A signed
Microsoft Store build is coming; until then, **More info → Run anyway** is how you
approve the app.
You can verify you downloaded the genuine file by checking its SHA-256 checksum,
which is published in each release's notes.

---

## Uninstalling

Trunkbase uninstalls like any Windows app:

1. Open **Settings → Apps → Installed apps** (or **Control Panel → Programs and
   Features**).
2. Find **Trunkbase** in the list, click the **⋯** menu, and choose
   **Uninstall**.
3. Follow the prompt to remove the application.

> _[Screenshot: the Windows "Installed apps" list with Trunkbase's ⋯ menu open
> and "Uninstall" highlighted.]_

**Your vault is not touched by uninstalling.** Your notes live in the folder you
chose, and they stay there. If you also want to delete your notes, remove that
vault folder manually afterward.

---

## Troubleshooting

| Problem | What to try |
|---|---|
| No **More info** link on the SmartScreen dialog | Your machine likely blocks unsigned apps by policy; a signed release is planned. |
| The app won't start after install | Reboot once, then relaunch. If it still fails, [open an issue](https://github.com/Ginamus/Trunkbase-releases/issues) with your Windows version. |
| First search seems stuck | The first search downloads a small model once; give it a minute on first use, then it's offline and fast. |
| I want to be sure the download is genuine | Compare the file's SHA-256 against the checksum listed in the [release notes](https://github.com/Ginamus/Trunkbase-releases/releases). |

Still stuck? [Open an issue](https://github.com/Ginamus/Trunkbase-releases/issues)
with a short description of what you did and what happened.
