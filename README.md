# orb — product page

The page served at **[t27.ai/orb/](https://t27.ai/orb/)**.

This repository holds the marketing page and nothing else. It is public so that
GitHub Pages can serve it: Pages is not available on a private repository under a
Free plan, which is the whole reason this is split out.

The application source is private, in `gHashTag/orb-app`, along with the releases.
Nothing here builds, signs or ships the app.

## How the domain works

`t27.ai` belongs to `gHashTag/ghashtag.github.io`. A user site's custom domain also
covers every other repository on the account, so a project site named `orb` is served
at `t27.ai/orb/` without knowing anything about the domain. `gHashTag/leela` reaches
`t27.ai/leela/` the same way.

## Editing

`landing.html` is standalone — no build step, no assets beyond Google Fonts. Open it
in a browser to work on it. Pushing to `main` deploys it.

The bubble in the hero is not an image. It is drawn in CSS with the same two-light
model the app uses — a violet key, a cyan bounce, one specular — and the halo buttons
change it live, so the page demonstrates the choice rather than describing it.

## Still to do

- Put a real checkout behind **Buy Orb**. It writes to admin@t27.ai for now, which
  reaches a human but does not take money.
- Ship a notarised build. Until then the DMG warns on any Mac but the one that built
  it, which is not something to charge $99 for.
