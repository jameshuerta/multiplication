# Blocks & Tables

A times-table trainer (up to 12 × 12) built on equal groups, arrays, skip counting, and place value. Single-file app; progress saves in the browser on-device.

## Deploy to Fly.io

One-time setup:

1. Push this repo to GitHub (branch: `main`).
2. If the app name `blocks-and-tables` is taken, change `app` in `fly.toml`.
3. Create the app once from your machine: `fly launch --no-deploy` (accept existing fly.toml), or `fly apps create blocks-and-tables`.
4. Generate a deploy token: `fly tokens create deploy -x 999999h`
5. Add it as a GitHub repo secret named `FLY_API_TOKEN` (Settings → Secrets and variables → Actions).

After that, every push to `main` deploys automatically. The app will live at `https://blocks-and-tables.fly.dev` (or your chosen name).

## iPad setup

Open the URL in Safari → Share → Add to Home Screen. Launches full screen with its own icon.

## Updating the app

Replace `index.html` and push. That's it.
