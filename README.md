# fogbound-site

The published pages for **Fogbound**, an iOS app.

**This repository is public on purpose, and holds nothing else.** The app's
source lives in a separate private repository. Keeping the two apart is the
point: a page that has to be served publicly should live somewhere that cannot
accidentally serve anything private alongside it. There is no build step and no
configuration that could widen what is published — the repository *is* the
website.

| file | what |
| --- | --- |
| `index.html` | landing page |
| `privacy.html` | the privacy policy — **the single copy**, and the one the App Store links to |
| `style.css` | shared styling, self-contained: no font host, no CDN, no analytics |

## Why the policy lives here and not with the app

It used to sit in the app repository as markdown. That is the wrong home for a
document whose whole purpose is to be published: it meant either two copies that
could drift, or a private file describing a public promise. A legal text that
says one thing in a repository and another on the web is worse than either.

So this is the source of truth. The app repository links to the live URL.

## Served by GitHub Pages

Settings → Pages → deploy from the `main` branch, root. No Jekyll needed; these
are plain files.

## Contact

`support.terra.app@proton.me` — a dedicated address rather than a personal one,
because this page is linked from an App Store listing and a listing outlives
anyone's interest in answering mail at the address on it.

The same address takes TestFlight feedback, so tester replies, App Review
correspondence and privacy enquiries all arrive in one place.
