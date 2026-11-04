# Load Forecaster — static site

A single-page app (`index.html`) that runs the `loadforecast` Python package in the
browser via Pyodide. No build step, no server, no database. Uploaded CSVs never leave
the visitor's browser.

## Deploy on Vercel

**Option A — from a computer (fastest)**

1. Install Node.js if needed, then in this folder run:
   ```
   npx vercel deploy --prod
   ```
2. Log in when prompted, accept the defaults ("Other" framework, no build command).
3. Vercel prints the public URL.

**Option B — from a browser or phone (GitHub + Vercel)**

1. On github.com create a new repository (e.g. `load-forecaster`), then
   "Add file → Upload files" and upload `index.html` (and this README). Commit.
2. On vercel.com: "Add New… → Project → Import" the repository.
3. Framework preset: **Other**. Leave Build Command and Output Directory empty. Deploy.
4. Vercel shows the URL, e.g. `https://load-forecaster.vercel.app`.

To update later, replace `index.html` (re-run Option A, or upload the new file to the
repo in Option B — Vercel redeploys automatically).

## Checking it works

Open the URL and wait 15–40 s on the first visit: the top card should change to
"✓ Python ready". The sample buttons work immediately either way.
