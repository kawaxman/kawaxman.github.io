# kentwaxman.life

Personal site. Plain HTML + CSS, no build step.

## Before publishing

1. Save the surf photo as `assets/hero.jpg` (export at ~2400px wide, JPEG quality ~80 so it stays under 500 KB).
2. Optionally drop your résumé at `assets/Kent-Waxman-Resume.pdf`, or remove the Résumé button in `index.html`.
3. Fix the dates and bullets in the Experience section (marked with a TODO comment).
4. Check the LinkedIn URL in the Contact section.

## Deploy to GitHub Pages

```bash
gh repo create kawaxman.github.io --public --source=. --push
```

Then in the repo: Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
The site goes live at https://kawaxman.github.io within a minute or two.

## Custom domain (kentwaxman.life)

1. Add a file named `CNAME` containing `kentwaxman.life` and push it.
2. At your DNS provider, add:
   - `A` records for `@` → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` record for `www` → `kawaxman.github.io`
3. In Settings → Pages, enter the custom domain and tick "Enforce HTTPS" once the certificate is issued.
