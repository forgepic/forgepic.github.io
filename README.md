# ForgePic frontend v1.0.1

Static GitHub Pages frontend for ForgePic.

Default deployment target in this build: `https://forgepic.github.io/`.
The public API URL is configured in `config.js` and defaults to `https://31.76.56.162/forgepic-api`.

No secret keys belong in the frontend.


## GitHub Pages deployment

Upload the contents of this archive directly to the root of the `forgepic/forgepic.github.io` repository.
Do not upload the ZIP itself or wrap the files in an extra directory.

GitHub Pages settings:
- Source: Deploy from a branch
- Branch: `main`
- Folder: `/ (root)`

Public site: `https://forgepic.github.io/`

## Backend CORS

The ForgePic API must allow the new frontend origin:

`https://forgepic.github.io`

If your backend `.env` currently contains another frontend origin, update ForgePic's own `ALLOWED_ORIGINS` / `FRONTEND_URL` values before testing login or generation.
Do not change CardForge configuration.
