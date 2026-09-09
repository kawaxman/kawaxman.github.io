# kentwaxman.com

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
The site goes live at https://kentwaxman.com within a minute or two.

## Custom domain (kentwaxman.com)

1. `CNAME` in the repo contains `kentwaxman.com`.
2. DNS lives in Vercel (`npx vercel dns ls kentwaxman.com`):
   - `A` records for `@` → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` record for `www` → `kawaxman.github.io`
3. Pages custom domain is set and HTTPS is enforced.
