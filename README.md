# Privacy policy — GitHub Pages

Live URL:

`https://alexchim1231.github.io/privacy/`

Public Pages repo: [AlexChim1231/AlexChim1231.github.io](https://github.com/AlexChim1231/AlexChim1231.github.io)

Edit source in this app repo: `privacy-site/privacy/index.html`  
Then deploy:

```bash
./scripts/deploy-privacy-github-pages.sh
```

Verify:

```bash
curl -sI https://alexchim1231.github.io/privacy/ | head -1
# expect: HTTP/2 200
```

`app.json` → `extra.privacyPolicyUrl` must match the live URL (no trailing path beyond `/privacy`).
