# deskfit-catalogue

Over-the-air content host for the **DeskFit** app (Channel B of its update system).

- `manifest.json` — `{ "version": N, "file": "catalogue.json", "minAppBuild"? }`. The app polls this.
- `catalogue.json` — the approved `[Stretch]` array the app caches.

Regenerate from the app repo with `scripts/publish-catalogue.py`, then commit here. Served via
GitHub Pages; the app reads its base URL from the `DeskFitCatalogueBaseURL` Info.plist key.
