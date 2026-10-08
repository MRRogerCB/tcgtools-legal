# tcgtools-legal — OBSOLETE (moved 8 Oct 2026)

> **This repository is no longer used.** Do not edit the policies here.
> Every page now redirects to its new home on **tcgtools.app**.

## Where the legal pages live now

| Document | Current URL |
|---|---|
| Privacy Policy | https://tcgtools.app/privacy |
| Terms of Service | https://tcgtools.app/terms |
| Account & Data Deletion | https://tcgtools.app/delete-account |

Use these URLs everywhere: Google Play Console (App content → Privacy
policy), App Store Connect (Privacy Policy URL), emails and support replies.

## How the pages are made and published

1. **Source of truth:** `lib/features/legal/legal_screens.dart` in the TCG Tools
   app repository (the same text the app shows in its own Legal screens).
2. **Generate:** run `py tools/build_legal_html.py` in the app repo. It writes
   `docs/html legal files/privacy.html`, `terms.html` and `delete-account.html`.
3. **Publish:** copy those files into the website repository (the site at
   tcgtools.app, under `/legal/`). Never hand-edit them there.

## What this repo still does

Only keeps old links working: `privacy.html`, `terms.html` and
`delete-account.html` here forward visitors (and search engines, via
`canonical` + `noindex`) to the URLs above. The old policy text remains in
this repository's git history.

Old URLs (now redirects):
- https://mrrogercb.github.io/tcgtools-legal/privacy.html
- https://mrrogercb.github.io/tcgtools-legal/terms.html
- https://mrrogercb.github.io/tcgtools-legal/delete-account.html

Once nothing links here any more, this repository can be archived on GitHub
(Settings → Danger Zone → Archive), which makes it read-only.
