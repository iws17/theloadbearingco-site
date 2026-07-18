# Site — The Load Bearing Co. (parked)

**URL:** http://theloadbearingco.com/  
**HTTPS:** GitHub is provisioning cert (enable when ready in repo Settings → Pages)  
**Repo:** https://github.com/iws17/theloadbearingco-site  
**Source:** `POD/site/index.html`

## Stack
- Static HTML on **GitHub Pages** (main branch `/`)
- DNS on **Cloudflare** (DNS only, not proxied):
  - `A @` → 185.199.108–111.153 (GitHub)
  - `CNAME www` → `iws17.github.io`
- Custom domain CNAME file in repo: `theloadbearingco.com`

## Why not CF Pages/Workers
Main API token lacked Pages/Workers edit. DNS token has zone DNS. GH Pages + CF DNS is the working path without expanding token sprawl.

## Edit / redeploy
```bash
cd ~/Projects/POD/site
# edit index.html
git add -A && git commit -m "update parked page" && git push
```

## Later
- Enforce HTTPS in GH Pages once cert exists
- Optional: orange-cloud proxy on CF after HTTPS stable
- Email MX when `hello@theloadbearingco.com` is ready
- Replace parked page with real shop when store is live
