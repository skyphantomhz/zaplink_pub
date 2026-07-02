# zapLink

**Share files over Wi-Fi between your computer and any phone or Smart TV — no cloud, no cables.**

🌐 **Website:** https://YOUR_GITHUB_USERNAME.github.io/zaplink/
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

1. **Create this repo as public** on GitHub (e.g. `zaplink`).
2. **Enable Pages:** Settings -> Pages -> Deploy from a branch -> `main` -> `/ (root)`.
3. **Edit `index.html`** and replace `YOUR_GITHUB_USERNAME` everywhere:
   - the download-button config (`OWNER` / `REPO`) near the bottom,
   - the SEO/social URLs in `<head>` (`canonical`, `og:url`, `og:image`, `twitter:image`, JSON-LD `url`).
   `OWNER`/`REPO` must point at **this public repo** so the download links resolve.
4. **Publish a release** here named `v1.0.0` and attach the three installer files.
   The page's buttons link to `releases/latest/download/<asset>`, so they always
   serve the newest release automatically.

See the private repo's `BUILD.md` for how the installers are built (PyInstaller
+ GitHub Actions).
