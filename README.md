# Game Glance PS5

A modified build of [Game Glance](https://github.com/michpalm/game-glance) (MIT, by Michael Palma) for Steam Deck Game Mode, installed through Decky Loader.

## Changes from the original
- Updates come from this repository, not the original one.
- Planned: PS5-style game page (square cover at the top, play button and game info along the bottom).

## Installing for the first time
In Decky: **Settings → Developer → Install Plugin from URL**:

```
https://github.com/BigHalalChickenProductions/game-glance-ps5/releases/latest/download/game-glance.zip
```

(or download `game-glance.zip` from Releases and use **Install Plugin from ZIP File**).

## Updating from the Deck
Quick Access menu → Game Glance → Updates. When a newer release exists it offers it; Decky asks you to confirm, installs it and reloads.

## Publishing a new version (browser only)
1. Change the files you need (usually `dist/index.js`).
2. Raise `version` in `package.json` (for example `3.6.4`).
3. Upload the changed files. You can upload in several goes: the `release` workflow waits 3 minutes, then builds `game-glance.zip` from everything on `main` and publishes release `v<version>`. If that version already has a release, nothing happens.

The updater only offers versions higher than the installed one, so always raise the number.

## Notes
- The repository must stay public so the Deck can read releases.
- Original license and third-party notices are kept in `LICENSE` and `THIRD_PARTY_LICENSES.md`.
