# tcgtools-legal

Public legal pages for the **TCG Tools** app (Polar Bear Studios), hosted via
GitHub Pages.

## Live URLs

The site is served from GitHub Pages at:

- **Landing / index:** https://mrrogercb.github.io/tcgtools-legal/
- **Privacy Policy:** https://mrrogercb.github.io/tcgtools-legal/privacy.html
- **Terms of Service:** https://mrrogercb.github.io/tcgtools-legal/terms.html
- **Account & Data Deletion:** https://mrrogercb.github.io/tcgtools-legal/delete-account.html

> The base URL pattern is `https://<username>.github.io/<repo-name>/<file>`.
> Here that's `mrrogercb` + `tcgtools-legal` + the page filename.

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page linking all three documents (main entry point). |
| `privacy.html` | Privacy Policy. |
| `terms.html` | Terms of Service. |
| `delete-account.html` | Account & data deletion instructions (Play-required URL). |

## Where these are used

- **In the app:** the in-app legal screens (`lib/features/legal/legal_screens.dart`)
  mirror this text. **The app's Dart text and these hosted pages must stay in
  sync** — treat them as one source of truth kept in two places.
- **Google Play Console:**
  - App content → Privacy policy → point at `privacy.html`.
  - App content → Data deletion → point at `delete-account.html`.

## Updating

1. Edit the relevant `.html` file(s).
2. Bump the "Effective date" / "Last updated" line in each edited file, and keep
   all three dates consistent when a change spans multiple docs.
3. Mirror any privacy/terms wording change into `legal_screens.dart` in the app.
4. Commit + push — GitHub Pages redeploys automatically within a minute or two.

## Notes

- Trademark/fan-content disclaimer appears at the bottom of privacy + terms.
  It's currently Pokémon-only; **each new TCG the app supports needs its own
  disclaimer added here and in the app** in the same release the game ships.
- These pages describe what the app does **today**. Planned features (e.g.
  cloud sync of decks) should not be described as if already live.

© 2026 Polar Bear Studios · TCG Tools · Jurisdiction: Mexico
