# NearbyPlay Static Site (GitHub Pages Ready)

This is a lightweight, production-ready static website for **NearbyPlay**.  
It includes:
- `index.html` (landing page with cards & lead form)
- `privacy.html`, `terms.html`
- `assets/styles.css`, `assets/logo.svg`

## 1) Preview locally
Just open `index.html` in your browser.

## 2) Deploy on GitHub Pages
1. Create a repo (e.g., `nearbyplay-site`) and upload all files.
2. In repo → **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` → `/root` → Save.
3. Your site will appear at `https://<your-username>.github.io/nearbyplay-site`.

## 3) Connect your Custom Domain on GitHub
1. In **Settings → Pages → Custom domain**, set: `www.nearbyplay.in` and **Enforce HTTPS**.
2. This creates a `CNAME` file automatically.
3. In **GoDaddy DNS**, set:
   - CNAME: `www` → `<your-username>.github.io`
   - Forward root: `nearbyplay.in` → `https://www.nearbyplay.in` (Permanent 301)
4. Wait a few minutes and test `https://www.nearbyplay.in`.

## 4) Lead Form (emails + logging)
This template uses **Formspree** as a zero-code email handler for static sites.

- Replace `YOUR_FORMSPREE_ID` in `index.html` with your endpoint from https://formspree.io (free tier available).
- Optional: Use **Zapier/Make** to pipe submissions into a **Google Sheet** automatically.

### Alternative (Netlify Forms)
If hosting on Netlify, replace the `<form>` tag with `data-netlify="true"` and add a hidden `form-name` field.

## 5) SEO & Meta
- Update `<meta>` tags in `index.html` to fine-tune title/description.
- Replace OpenGraph image if desired.

## 6) Content Edits
- Update company details inside `index.html`, `privacy.html`, `terms.html`.
- Colors and typography live in `assets/styles.css`.

---

© 2025 NearbyPlay Technologies Private Limited. All Rights Reserved.