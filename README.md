# ENPHITIC Build Plan tracker

A single-page app with every step from the founders' agreement to the App Store and Google Play. Tick a step and it records who did it (Trevor or Victor) and when. Progress is saved in `progress.json` in this repository, so both founders see the same plan.

## Put it online (GitHub Pages)

1. Create a new repository, e.g. `enphitic-tracker`.
2. Upload `index.html` and this `README.md` to the root of the `main` branch.
3. Go to the repository's Settings, then Pages. Under "Build and deployment", choose "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
4. After a minute the tracker is live at `https://<owner>.github.io/enphitic-tracker/`.

Note: GitHub Pages on a private repository needs a paid GitHub plan. On the free plan the repository (and the plan in it) is public.

## Turn on shared sync (each founder, once)

1. On GitHub, create a fine-grained personal access token:
   - Repository access: only `enphitic-tracker`
   - Permissions: Contents, Read and write
2. Open the tracker, click "Sync settings", enter the repository (`owner/enphitic-tracker`), branch `main`, file `progress.json` and your token.
3. Click "Test connection", then "Save and sync".

The token stays in your browser only. `progress.json` is created on the first save. The app checks for the other founder's changes every 30 seconds and merges them automatically.

## Adding steps

- Quick: use "Add a step" at the end of any section in the app. It syncs like everything else.
- Permanent: edit the `PLAN` list at the top of the script in `index.html`. Add new steps at the end of a section, because each step's ID comes from its position.

## Backup

"Sync settings" has "Download backup" and "Restore from file".
