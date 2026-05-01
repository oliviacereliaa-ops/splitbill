# Split Bill

A static web app that splits a restaurant/group bill from a receipt photo. Upload a photo, OCR runs in your browser (Tesseract.js), then assign items to people. Tax/service/tip applied proportionally. No server, no data leaves the device.

## Features

- Receipt photo upload + client-side OCR (Tesseract.js, English)
- Manual item entry as a fallback
- Add people, assign items (incl. shared items split among multiple people)
- Tax / Service / Tip as percentages
- Per-person totals + grand total

## Run locally

Just open `index.html` in a browser. No build step.

## Deploy to GitHub Pages

1. Create a new repo on GitHub and push these files:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
2. On GitHub → **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. The included workflow (`.github/workflows/deploy.yml`) auto-publishes on every push to `main`.
4. Your site will be live at `https://<your-username>.github.io/<your-repo>/`.

## Tech

- Plain HTML/CSS/JS (single file)
- [Tesseract.js v5](https://tesseract.projectnaptha.com/) loaded from CDN

## License

MIT
