# Megalith — support site

Static site served via **GitHub Pages** for the [Megalith](https://apps.apple.com/) iOS app. It provides the two URLs App Store Connect requires:

| App Store Connect field | URL |
|---|---|
| **Support URL** | `https://lukebradford.github.io/megalith/` |
| **Privacy Policy URL** | `https://lukebradford.github.io/megalith/privacy.html` |

## Files

- `index.html` — support page (about, how to use, contact, privacy summary, hero screenshot)
- `privacy.html` — full privacy policy
- `wordmark.svg` — the "MEGALITH" wordmark (Superclarendon Bold, glyphs outlined so no font is shipped)
- `because.png` — app screenshot shown in the hero (iPhone frame is pure CSS)
- `AppIcon.png`, `apple-touch-icon.png` — favicon / touch icon (black serif "M" on amber)
- `.nojekyll` — serve files as-is (skip Jekyll processing)

## Publish

```bash
# from this directory, after creating an empty github.com/lukebradford/megalith repo
git remote add origin git@github.com:lukebradford/megalith.git
git push -u origin main
```

Then in the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `/ (root)`**. The site goes live at `https://lukebradford.github.io/megalith/` within a minute or two.

To preview locally:

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
