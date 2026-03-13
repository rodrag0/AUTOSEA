# AUTOSEA

Website for AUTOSEA.

## Deploy on Vercel

This repo is a static site (HTML + images), so Vercel can deploy it without a build step.

### Option 1: Deploy from GitHub (recommended)
1. Push this repository to GitHub.
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo.
3. Framework preset: **Other**.
4. Leave build settings empty:
   - Build Command: *(empty)*
   - Output Directory: *(empty)*
5. Click **Deploy**.

The repo now includes `index.html`, which Vercel serves automatically as the homepage.

### Option 2: Vercel CLI
1. Install CLI:
   ```bash
   npm i -g vercel
   ```
2. From this project folder, run:
   ```bash
   vercel
   ```
3. For production deployment:
   ```bash
   vercel --prod
   ```

### Notes
- Keep these files in the repo root so relative image paths continue to work:
  - `index.html`
  - `autosea_esa_pwp.html`
  - `Background.png`
  - `LM450_Details.jpg`
  - `PXL_20260106_120113268.jpg`
  - `lm450-101-hull-sw-surface_v17.glb`


### 3D model section
- The interactive vessel section loads `lm450-101-hull-sw-surface_v17.glb` with the `model-viewer` web component from unpkg.
