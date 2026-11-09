# ismailmarketing.com

Static site (HTML/CSS/JS). No build step needed to host it.

## Before you publish
1. Open `_build/build.py`, set `WA_NUMBER`, `PHONE_DISPLAY`, `EMAIL`, `LOCATION_LINE`, `SOCIALS`, and (when ready) `GA4_ID` / `GSC_VERIFY`.
2. Run `python3 _build/build.py` to regenerate every page. (Edit copy in `_build/content.py`.)
3. Preview locally: `python3 -m http.server 8000` then open http://localhost:8000

## Deploy on GitHub Pages
1. Push this folder to a repo, then Settings > Pages > Deploy from branch (main, root).
2. Custom domain: `ismailmarketing.com` (the `CNAME` file is included). Tick "Enforce HTTPS".
3. DNS at your registrar: four A records for the apex pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153, and a CNAME for `www` pointing to `<your-github-username>.github.io`.
4. In Google Search Console add the domain and submit `https://ismailmarketing.com/sitemap.xml`.
