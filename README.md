# Privacy policy and support — GitHub Pages

Public Pages repo: [AlexChim1231/AlexChim1231.github.io](https://github.com/AlexChim1231/AlexChim1231.github.io)

Live URLs:

- Privacy policy: `https://alexchim1231.github.io/privacy/`
- Support: `https://alexchim1231.github.io/support/`

Edit this repository directly:

- `privacy/index.html`
- `support/index.html`

GitHub Pages serves each folder’s `index.html` at that path with or without a trailing slash. The site root `index.html` redirects to the privacy policy.

Verify:

```bash
curl -sI https://alexchim1231.github.io/privacy/ | head -1
# expect: HTTP/2 200

curl -sI https://alexchim1231.github.io/support/ | head -1
# expect: HTTP/2 200

curl -s https://alexchim1231.github.io/robots.txt
# expect: User-agent: * with Allow: /

curl -s https://alexchim1231.github.io/app-ads.txt
# expect: google.com, pub-… line
```

`app.json` → `extra.privacyPolicyUrl` must match the live privacy URL (no trailing path beyond `/privacy`).
