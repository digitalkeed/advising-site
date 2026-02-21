# Advising.com

Static landing page. Deploy to Vercel by connecting this repo.

## Deploy on Vercel

1. Push this folder to a new GitHub repo (see below).
2. Go to [vercel.com](https://vercel.com) → **Add New** → **Project**.
3. **Import** your GitHub repo.
4. Leave **Framework Preset** as "Other" (or "Vite" doesn’t matter for static HTML).
5. **Root Directory**: `.` (default).
6. Click **Deploy**. Your site will be live at `https://your-project.vercel.app`.

---

## Push to GitHub (first time)

From your Mac, in Terminal:

```bash
cd /Users/test/advising-site

# Create repo on GitHub first: github.com → New repository → name it e.g. "advising-site" (no README, no .gitignore)

git init
git add .
git commit -m "Initial commit: Advising.com landing page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/advising-site.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username and `advising-site` with your repo name.

**Note:** The page uses image URLs from Figma’s API. Those may not load for everyone once deployed. For a production site, export images from Figma and host them in the repo or on a CDN, then update the `src` and `background-image` URLs in `index.html`.
