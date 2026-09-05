# terra-incognita-site

The published pages for **Terra Incognita**, an iOS app.

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

## Before publishing

`privacy.html` carries a highlighted **ADD A CONTACT ADDRESS BEFORE PUBLISHING**
placeholder. A privacy policy needs a working contact, and a personal address on
a public page invites spam — a dedicated one is the cheap answer.
