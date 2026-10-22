# ENPHITIC Studio Roadmap

Every tech and development step for ENPHITIC Studio, from the first design decision to the App Store and Google Play. Tick a step and it records who did it (Trevor or Victor) and when. Progress is saved in `progress.json` in this repository so both of you see the same plan.

## Files
- `index.html` — the app
- `manifest.webmanifest`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `favicon-32.png` — home screen icon and app settings

Upload all of them to the root of the repository.

## Turn on the website
Settings → Pages → Deploy from a branch → `main`, `/ (root)` → Save.
Live at `https://enphitic-hash.github.io/studio_roadmap/`.

## Add to your iPhone home screen
Open the link in Safari → Share → Add to Home Screen. It opens full screen with the ENPHITIC E icon, like an app.

## Turn on sync (each of you, once per device)
1. GitHub → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate.
2. Repository access: only `studio_roadmap`. Permission: Contents, Read and write.
3. In the app: Settings → paste the token → Test connection → Save and sync.

## Adding steps
Use "Add" at the end of any section in the app, or edit the `PLAN` list in `index.html`. Step IDs come from step titles, so renaming a step resets its tick.
