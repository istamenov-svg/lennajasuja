# Lenna Jasuja — Personal Website

Single-page personal site for Lenna Jasuja.

## GitHub Pages Setup

1. Create a new repo (e.g. `lennajasuja.github.io` or any name)
2. Push all files from this folder to the repo root
3. Go to **Settings → Pages → Source** and select the `main` branch
4. The site will be live at `https://<username>.github.io/<repo-name>/`

## Custom Domain

Once a domain is purchased:

1. In the repo, go to **Settings → Pages → Custom domain** and enter the domain
2. Add these DNS records with the domain registrar:
   - **A records** pointing to GitHub's IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **CNAME record**: `www` → `<username>.github.io`
3. Check "Enforce HTTPS" in the Pages settings
4. GitHub will auto-generate a `CNAME` file in the repo

## File Structure

```
├── index.html          # The full single-page site
├── images/
│   └── headshot.jpg    # Lenna's headshot photo
└── README.md
```

## Updating Content

Everything is in `index.html` — plain HTML/CSS/JS, no build tools needed. Edit directly and push.
