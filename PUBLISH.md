# Publishing the new site at launchriot.online
## Current hosting (checked 15 Oct 2026)
- DNS: A launchriot.online = 34.111.179.208 (Google Cloud front end); nameservers hermes/artemis.dns-parking.com (Hostinger DNS); MX/SPF = Hostinger mail. www has no record (NXDOMAIN).
- HTTP: `server: Google Frontend`, `GAESA` cookie, Vite/React SPA, served via Google (Hostinger Horizons-style hosting, not GitHub Pages).
- Domain is therefore managed in Hostinger; the site content is deployed through whatever tool produced the Vite app.
## To publish
1. Decide: (a) replace the content in the current host (upload this static folder / redeploy), or (b) move to GitHub Pages: add CNAME file `launchriot.online`, set Hostinger A records to 185.199.108.153/.109.153/.110.153/.111.153 (replace 34.111.179.208), add CNAME `www` -> cliffordlandman-alt.github.io, enable HTTPS in Pages settings. Keep MX/TXT records untouched.
2. Option (b) needs Clifford/Hostinger access and causes brief cutover; email records must not change.
3. GitHub Pages terms restrict commercial SaaS hosting; a static marketing page is fine, the product itself should move later.
4. Before go-live: link adviser demo (currently 404), confirm contact details, add favicon check, re-run QA.
