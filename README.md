# ashachokshi.art — Coming Soon

Static coming soon page for [ashachokshi.art](https://ashachokshi.art).

## Deploy to GitHub Pages

1. Initialize the repo and push:
   ```bash
   git init
   git add .
   git commit -m "Add coming soon page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/asha-art-portfolio.git
   git push -u origin main
   ```

2. In the GitHub repo go to **Settings → Pages → Source** and select `main` branch, `/ (root)`.

3. GitHub will give you a URL like `https://<username>.github.io/asha-art-portfolio`. Verify it loads.

## Point ashachokshi.art to GitHub Pages

Add these DNS records at your domain registrar:

| Type  | Name | Value                    |
|-------|------|--------------------------|
| A     | @    | 185.199.108.153          |
| A     | @    | 185.199.109.153          |
| A     | @    | 185.199.110.153          |
| A     | @    | 185.199.111.153          |
| CNAME | www  | `<username>.github.io`   |

Then in GitHub Pages settings set **Custom domain** to `ashachokshi.art` and enable **Enforce HTTPS** once the certificate provisions (can take up to 24 hours).

## Swap in real artwork

Replace the placeholder `<div class="artwork-placeholder">` in `index.html` with:

```html
<img src="artwork.jpg" alt="Painting by Asha Chokshi" class="artwork-placeholder" />
```

Add the image file to the repo root and push.
