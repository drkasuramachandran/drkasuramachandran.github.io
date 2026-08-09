# Deploying to GitHub Pages (free, no monthly cost)

## 1. One-time setup on GitHub
1. Go to github.com and create a **new repository** — name it anything, e.g. `portfolio`.
   - Keep it **Public** (required for free GitHub Pages).
   - Don't add a README when creating it.
2. On the repo page, click **"uploading an existing file"** (or use the Add file → Upload files button).
3. Drag in these three items exactly as they are:
   - `index.html`
   - the `assets` folder (with `headshot.jpeg` and `Ramachandran_Kasu_CV.pdf` inside)
4. Commit the files (green "Commit changes" button).

## 2. Turn on Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment", set **Source: Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Save.
4. GitHub will give you a URL like `https://yourusername.github.io/portfolio/` within a minute or two.

## 3. Point your domain at it
Since you already own a domain, in your domain registrar's DNS settings:

**Option A — apex domain (e.g. `drkasuramachandran.com`):**
Add four **A records** pointing `@` to GitHub's Pages IPs:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Option B — subdomain (e.g. `www.drkasuramachandran.com`):**
Add a **CNAME record**: `www` → `yourusername.github.io`

Then in your GitHub repo, go to **Settings → Pages → Custom domain**, type your domain, and save. GitHub will auto-provision a free HTTPS certificate (can take up to 24 hours).

## 4. Updating content later
Just edit `index.html` directly on GitHub (pencil icon) or re-upload the file — changes go live within a minute, no redeploy step needed.

---

### A couple of things to fill in before/after publishing
- **Google Scholar / secondary email**: if you'd like either added, just let me know and I'll wire them in.
