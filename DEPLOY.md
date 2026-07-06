# Deploying to GitHub Pages — 2 minutes

## Option A · New repository (recommended)
1. On github.com: **New repository** → name it e.g. `apexfusion-site` → Public → Create.
2. On the empty repo page, click **"uploading an existing file"**.
3. Drag in ALL files from this folder: `index.html`, `vector.html`, `token.html`, `foundation.html`, `styles.css`.
4. Commit directly to `main`.
5. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
6. Live in ~1 minute at: `https://<your-username>.github.io/apexfusion-site/`

## Option B · Command line
    git clone https://github.com/<you>/apexfusion-site.git
    cp *.html styles.css apexfusion-site/
    cd apexfusion-site && git add . && git commit -m "Apex Fusion site v2" && git push
Then enable Pages as in step 5 above.

## Custom domain (apexfusion.org)
Settings → Pages → Custom domain → enter domain → add the DNS records GitHub shows
(A records for apex domain, CNAME for www) at your registrar. HTTPS auto-provisions.

## Before going public — fix these placeholders
- [ ] CEO surname in index.html + foundation.html ("Christopher [Surname]")
- [ ] Verify the publicly-announced leadership roster
- [ ] Real URLs for: Docs, MCP server, Explorer, GitHub, Whitepaper, Contact (currently "#")
- [ ] CLI syntax in the terminal blocks (marked illustrative)
- [ ] Confirm current exchange listings on token.html
