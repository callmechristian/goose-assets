# goose-assets

Shared icons, logos, and marketing assets for the Goose app flock.

Each app consumes this repo as a git submodule and runs its own sync script to copy the files it needs.

## Structure

- `icons/` — app icons, favicons, maskable icons
- `logos/` — wordmarks, written logos, short logos
- `marketing/` — screenshots, hero images, social cards
- `source/` — PSDs, AI files, and other working files (Git LFS)

## Naming

Use per-app prefixes so each file is unambiguous:

- `nibbl-logo-written.png`
- `repr-appico.png`

## Adding a new app

1. Add the required assets under `icons/` and `logos/` using the app name as a prefix.
2. In the app repo, add `goose-assets` as a submodule and wire up `scripts/sync-assets.mjs`.
