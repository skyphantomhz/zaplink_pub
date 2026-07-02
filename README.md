# zapLink

**Share files over Wi-Fi between your computer and any phone or Smart TV — no cloud, no cables.**

🌐 **Website:** https://skyphantomhz.github.io/zaplink_pub/
⬇️ **Downloads:** see the [Releases](../../releases/latest) page.

zapLink turns your computer into a private local server. Pick a folder, hit
Start, and any device on the same Wi-Fi opens it in a browser — protected by a
PIN. Free for **macOS, Windows and Linux**.

---

## This repository

This is the **public landing page + downloads** for zapLink:

- `index.html` — the marketing site, served via GitHub Pages.
- `static/` — the share image and icons used by the page.
- **Releases** — the installer downloads (`zapLink-macos.zip`,
  `zapLink-windows.zip`, `zapLink-linux.tar.gz`).

The application source code lives in a separate (private) repository.

---

## Maintainer setup

Already configured for **skyphantomhz/zaplink_pub**.

1. Push this repo to `git@github.com:skyphantomhz/zaplink_pub.git`.
2. **Enable Pages:** Settings -> Pages -> Deploy from a branch -> `main` -> `/ (root)`.
   Site goes live at https://skyphantomhz.github.io/zaplink_pub/
3. **Publish a release** named `v1.0.0` and attach the three installer files
   (`zapLink-macos.dmg`, `zapLink-windows-setup.exe`, `zapLink-linux-x86_64.AppImage`).
   The page's download buttons link to `releases/latest/download/<asset>`, so
   they always serve the newest release automatically.

The installers are built from the private source repo (see its `BUILD.md`) —
either published here automatically via CI (PAT) or uploaded manually.

