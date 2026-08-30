# animeshprakash.com — premium build

Single-page personal site. No build step, no dependencies to install — `index.html` is
self-contained (all CSS and JS inline; only Google Fonts is loaded externally).

## Files

| File | Purpose |
|---|---|
| `index.html` | The site |
| `404.html` | Branded not-found page |
| `avatar.webp`, `portrait.webp`, `board-portrait.webp` | Photography (hero avatar, hero portrait, Board & Advisory portrait) |
| `og-image.png` | 1200×630 share card (LinkedIn, WhatsApp, X, Slack previews) |
| `robots.txt` | Search-engine directives |
| `sitemap.xml` | Sitemap |
| `netlify.toml` | www → apex redirect + security headers |
| `_headers` | Same headers, fallback format |

## Deploy (either way — 2 minutes)

**A. GitHub (keeps auto-deploy):**
1. Open `github.com/animeshprakashfrance/animeshprakash-portfolio`
2. **Add file → Upload files**, drag in all files above
3. **Commit changes** — Netlify rebuilds and publishes automatically

**B. Netlify drag-and-drop:**
1. Netlify → your site → **Deploys**
2. Drag this whole folder onto the drop area

DNS and Zoho email are untouched by either route.

## Editing later

Everything is plain text in `index.html`. Content sits after `</style>`; the design
tokens (colours, spacing) are the `:root` variables at the top of the `<style>` block.

## Notes

- The "Save as PDF / CV" button in the footer prints the page through a dedicated
  print stylesheet — clean, one-column, no nav or decoration.
- `og-image.png` must sit at the site root for social previews to resolve.
- After deploying, refresh LinkedIn's cache with the Post Inspector so the new
  share card shows: linkedin.com/post-inspector
