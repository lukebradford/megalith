# Megalith — support site

Static site served via **GitHub Pages** for the [Megalith](https://apps.apple.com/) iOS app. It provides the two URLs App Store Connect requires:

| App Store Connect field | URL |
|---|---|
| **Support URL** | `https://lukebradford.github.io/megalith/` |
| **Privacy Policy URL** | `https://lukebradford.github.io/megalith/privacy.html` |

## Files

- `index.html` — support page (about, how to use, contact, privacy summary)
- `privacy.html` — full privacy policy
- `AppIcon.png`, `apple-touch-icon.png` — app icon (black serif "M" on amber)
- `league.otf` — League Gothic, the display font used for the wordmark
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
