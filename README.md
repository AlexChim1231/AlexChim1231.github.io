# Privacy policy — GitHub Pages (this repo)

Live URL (project Pages):

`https://alexchim1231.github.io/BEYBLADE-BATTLE-APPS/privacy/`

Source of truth for edits: `privacy-site/privacy/index.html`  
Published copy: `docs/privacy/index.html` (GitHub Pages serves `/docs` from `main`)

## Deploy

```bash
./scripts/deploy-privacy-github-pages.sh
git add docs privacy-site
git commit -m "docs: update privacy policy page"
git push origin main
```

Then confirm:

```bash
curl -sI https://alexchim1231.github.io/BEYBLADE-BATTLE-APPS/privacy/ | head -1
# expect: HTTP/2 200
```

`app.json` → `extra.privacyPolicyUrl` must match the live URL above.
