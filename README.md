# Banting website

Static site for https://bantingapp.github.io/ (GitHub Pages). Plain HTML plus one shared stylesheet (`banting.css`). No build step, no JavaScript. `.nojekyll` tells GitHub Pages to serve the files as they are.

**These texts are drafts.** Have a qualified person (a lawyer or privacy professional familiar with GDPR, POPIA and consumer law) review the privacy policy, terms and deletion page before launch.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Short intro, links to all pages, "Coming soon to Google Play" |
| `privacy.html` | Privacy policy (use this URL in Google Play and in the app) |
| `terms.html` | Terms of use |
| `delete-account.html` | Account and data deletion page (URL required by Google Play Data safety) |
| `contact.html` | Support contact |

## Placeholders to replace

Search the whole folder for `[[` and replace each value. Nothing else is owner-specific.

| Placeholder | Meaning | Appears in |
| --- | --- | --- |
| `[[OWNER_NAME]]` | Your legal name or business name | `privacy.html` (sections 1, 14), `terms.html` (section 1), `delete-account.html` (intro), `contact.html` (bottom) |
| `[[OWNER_COUNTRY]]` | Country you are based in | `privacy.html` (sections 1, 8, 14), `terms.html` (section 1), `contact.html` |
| `[[SUPPORT_EMAIL]]` | Real support email address (used as text and in `mailto:` links) | every page except `index.html`; the deletion button in `delete-account.html` also uses it |
| `[[GOVERNING_LAW]]` | Governing law, for example "England and Wales" (decide with your adviser) | `terms.html` section 13 |

After replacing, delete the yellow `.ph` highlight rule at the bottom of the "Placeholder highlight" comment in `banting.css`.

## Check before publishing

- Effective date is 9 November 2026 in `privacy.html` and `terms.html`. Update it if you publish later or change the text.
- The app must really do what the policy says: explicit health-data consent screen, Google UMP consent form (with a way to change the choice), no health data sent to AdMob, Facebook advertiser ID and auto event logging off, Delete account in Profile.
- Replace the in-app placeholder links (`PRIVACY_POLICY_URL`, `TERMS_URL`, `SUPPORT_EMAIL`) with these pages.


## Filled in (9 Nov 2026)
OWNER_NAME = Magdalena Ivanovska · OWNER_COUNTRY = North Macedonia · SUPPORT_EMAIL = fitnfoods@gmail.com · GOVERNING_LAW = the Republic of North Macedonia. The placeholders have been replaced in all pages.
