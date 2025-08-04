# OEF DCS Mission Repository

This repository hosts DCS mission files with automatic version tracking and CDN distribution.

## Setup Instructions

1. Create a new repository on GitHub
2. Add this repository as the remote origin:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/oefmiz.git
   ```
3. Push to GitHub:
   ```bash
   git branch -M main
   git push -u origin main
   ```
4. Enable GitHub Pages:
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: `gh-pages` (will be created automatically)

## How It Works

- Push updated `.miz` files to trigger automatic releases
- GitHub Actions creates versioned releases with timestamps
- `missions.json` is updated automatically and served via GitHub Pages
- Your website can fetch mission data from: `https://YOUR_USERNAME.github.io/oefmiz/missions.json`

## Mission Naming Convention

Use the format: `OEF_169_vX.Y.Z.miz` where X.Y.Z is the version number.