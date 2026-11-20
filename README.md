# Mert Lafcı — Portfolio

Single-page bilingual (EN / TR) personal site for **Mert Lafcı**, independent developer. One `index.html` plus an `assets/` folder for screenshots. No build step, no framework.

## What’s on the page

- Hero: name, "Independent Developer", short intro
- **Projects**
  - Meridyen Terapi Asistanı (App Store + Google Play)
  - HiFi Companion (macOS, open source; GitHub + latest release)
  - PocketPaste (Android → Mac, open source; GitHub + latest release)
- **How I work**: AI-assisted development workflow
- **Contact**: email, GitHub, LinkedIn
- Language toggle (EN default, TR available; `?lang=tr` works; choice saved in `localStorage`)

Screenshots live in `assets/`, copied from each app's repo.

## Open locally

**Option A — open the file**

```bash
open index.html
# or double-click index.html in your file manager
```

**Option B — tiny static server**

```bash
# Python
python3 -m http.server 43127

# or Node (if you have npx)
npx --yes serve -l 43127
```

Then visit [http://127.0.0.1:43127](http://127.0.0.1:43127).

Fonts load from Google Fonts (Fraunces + DM Sans); CSS and JS are inline in `index.html`, images are in `assets/`.
