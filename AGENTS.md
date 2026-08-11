# Casimir Cleaning public site — agent rules

This standalone nested Git repository is the PUBLIC product site. It is not the
internal Casimir Cleaning manager.

## Identity and boundaries

- Public source: `C:/trio/Projects/casimir_cleaning_public`
- Public repo: `scasimir2021/casimir-cleaning`, branch `main`
- Live URL: `https://scasimir2021.github.io/casimir-cleaning/`
- Internal app source: `C:/trio/Projects/casimir_cleaning`
- Internal live app: pc-black `:4081`, systemd `casimir-cleaning`

Never copy internal clients, addresses, invoices, notes, schedules, database
files or client photos into this repository. Never publish LAN addresses
(`10.10.10.*`), tailnet hostnames (`*.ts.net`), or any token.

The hero "screenshot" is hand-written markup, deliberately: a real screenshot of
the app risks shipping client data. Keep it that way — if you refresh it, edit
the markup, do not paste an image of the live app.

## Editing

- Copy and layout: `index.html`. Palette and layout: `assets/css/site.css`.
- Keep the palette in step with the app (`--navy #1B3A5C`, `--accent #4A90D9`).
- Verify locally (`python -m http.server 4182 --bind 127.0.0.1`) before pushing.
- Pricing is deliberately "ask and we will quote it" — do not invent a number
  without Steven's say-so.
- Push `main`; the Pages workflow deploys. Confirm the live URL afterwards.
