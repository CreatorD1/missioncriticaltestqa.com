# Mission Critical Test QA — GitHub Pages site

`index.html` is the full landing page, exported from the Muse artifact. Push-ready as-is.

## Publish free on GitHub Pages

1. Create a **public** GitHub repo, e.g. `missioncriticaltestqa`
2. Upload `index.html` to the repo root (drag & drop on github.com works fine)
3. Repo → **Settings → Pages** → Source: *Deploy from a branch* → branch `main`, folder `/(root)` → Save
4. Live in ~1–2 min at `https://<your-username>.github.io/missioncriticaltestqa`

## Use your own domain (missioncriticaltestqa.com)

1. In the repo: **Settings → Pages → Custom domain** → enter `missioncriticaltestqa.com` → Save (GitHub creates the `CNAME` file for you)
2. At your domain registrar's DNS settings:
   - Four `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record for `www` → `<your-username>.github.io`
3. Wait for DNS to propagate (up to 24h), then tick **Enforce HTTPS** in Pages settings

## Notes

- The Calendly booking embed is **not** on the page yet — send the Calendly URL and it will be added, then this file re-exported.
- After any page update, re-export from the artifact and replace `index.html`, then push.
