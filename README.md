# Vision

> "Where there is no vision, the people perish." — Proverbs 29:18

A personal vision app built around a hub: one view that says, plainly, *these are the
vision targets, this is what we are going after* — with every goal anchored to one of them.

This app is the consolidation of two earlier apps. **Vision** held the vision, the values
and the pursuits. **Orbit** ([`goals-app`](https://github.com/claudekovalenko/goals-app))
tracked goals in concentric tiers. They are now one thing, because they were always about
the same question: what is central, and what is merely near it?

## The hub

The hub is the centre of the app, not a feature of it.

- **The centre** — remaining in Jesus (John 15). Everything else radiates from it.
- **The gold ring** — the **vision targets**: what the Lord has made central. These are
  the things being run after.
- **Small gold circles** — the **goals in pursuit of each target**, drawn as moons around
  the target they serve, joined to it by a line. Finished goals turn green.
- **Blue ring** — ancillary pursuits. Good, but not the centre.
- **Dashed outer circles** — **unanchored goals**: goals tied to nothing central. The map
  shows them adrift on purpose, with no line home. Anchor them, or let them go.

Click any circle to open it: rename it, edit the note, tick goals off, add a goal, move a
pursuit between central and ancillary. Selecting something dims everything unrelated, so
one target and its goals can be looked at on their own.

## The rest

- Editable vision statement, held in light of eternity
- **Values** — the marks of the culture being built
- **Vision targets (central)** and **ancillary** pursuits, each holding its own goals
- **Unanchored goals** — surfaced as their own section whenever any exist
- **Vehicles** — the concrete means and structures the vision moves through
- **Dreams held lightly** — senses and impressions, carried with open hands
- **My gifts** — how God has wired you, so pursuits trace back to gifting
- **Decision filter** — test a decision against remaining in Jesus, each vision target,
  and your gifts, for an alignment read-out
- Export and import a JSON backup

Everything saves automatically to your browser (localStorage). No server, no build step,
no accounts.

## Coming from the old apps

Nothing needs moving by hand. On first load the app carries over:

- your saved **Vision** data (`vision-app-v2`, and the older `vision-app-v1`), and
- your **Orbit** goals (`orbit-goals-v1`), which arrive unanchored so you can tie each one
  to a target.

Both apps are served from the same origin on GitHub Pages, so their stored data is
readable here. If you used Orbit somewhere else — another domain, or a local file — export
from Orbit and use **Import a backup** at the bottom of this page; a plain Orbit goals
export is recognised and folded in as unanchored goals.

## Running it

A single static file. Open `index.html` in a browser, or serve the folder:

```sh
npx serve .
```

## Install as an app (PWA)

Served over HTTPS (e.g. GitHub Pages) it installs like an app:

- **Phone** — open the site, then "Add to Home Screen"
- **Desktop** — the install icon in the address bar

It works offline after the first visit; a service worker caches the app and everything
lives in localStorage.
