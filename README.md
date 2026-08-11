# Casimir Cleaning — public product site

Marketing landing page for the Casimir Cleaning business manager. Static HTML +
one stylesheet, no build step, no JavaScript.

- **Live:** https://scasimir2021.github.io/casimir-cleaning/
- **Source of truth:** `C:/trio/Projects/casimir_cleaning_public` on dev-desktop
- **Deploy:** push `main` → GitHub Actions Pages workflow (`.github/workflows/pages.yml`)
- **The product it sells:** `C:/trio/Projects/casimir_cleaning` (internal app, pc-black `:4081`)

```
index.html              the whole page
404.html                not-found page (absolute /casimir-cleaning/ paths)
assets/css/site.css     palette + layout
assets/brand/logo.svg   sparkle mark, same as the app favicon
assets/brand/social.svg og:image card
```

## Editing

Check locally before pushing:

```powershell
python -m http.server 4182 --bind 127.0.0.1   # then open http://127.0.0.1:4182/
```

The dashboard mock in the hero is hand-written markup that mirrors the real app's
layout and palette — it is not a screenshot, so it never contains client data.
If the app's palette changes, update `:root` here to match.

## Boundaries

This repository is public. It must never contain client names, addresses,
invoices, photos, database files, tokens, or internal URLs (`10.10.10.*`,
`*.ts.net`). Contact details on the page are Steven's already-public business
phone and email.
