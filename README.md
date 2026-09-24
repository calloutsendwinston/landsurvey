# Calloutsend

Static one-page site (`index.html`, no build step) for Calloutsend — land survey and property development.

## 1. Push to GitHub

Create an empty repo on GitHub first (no README/license, so there's nothing to merge), then:

```bash
cd calloutsend-site
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/calloutsend.git
git push -u origin main
```

## 2. Deploy on Vercel

**Option A — connect the GitHub repo (auto-deploys on every push):**
1. vercel.com → New Project
2. Import the `calloutsend` repo
3. Framework preset: "Other" — leave build/output settings blank, there's nothing to build
4. Deploy

**Option B — deploy straight from your machine, no GitHub needed:**
```bash
npm i -g vercel
cd calloutsend-site
vercel
```
Follow the prompts; you'll get a live `*.vercel.app` URL.

## 3. Custom domain

Once deployed, go to the project's **Settings → Domains** in Vercel, add your domain (e.g. `calloutsend.com`), and follow the DNS records it gives you.
