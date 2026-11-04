# sevenoaks.digital

The company website for Seven Oaks Digital, L.L.C. — a single static page served by GitHub Pages at <https://sevenoaks.digital>.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole site: semantic HTML with inline CSS. No JavaScript, no build step. |
| `favicon.svg` | Star favicon. |
| `CNAME` | Tells GitHub Pages to serve the site at `sevenoaks.digital`. |
| `.nojekyll` | Serve files as-is (skip Jekyll processing). |

## Rules

- No cookies, analytics, tracking, forms, or third-party requests (fonts, CDNs, scripts). This keeps the site free of any need for a cookie banner.
- Public contact address is `hello@sevenoaks.digital` only.
- Must stay responsive at 375 px, support light and dark mode via `prefers-color-scheme`, and meet WCAG AA contrast.

## Preview locally

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy

GitHub Pages deploys from the `main` branch root. In the repo's **Settings → Pages**, set the source to `main` / `(root)` and the custom domain to `sevenoaks.digital`, then turn on **Enforce HTTPS** once the certificate is issued.

DNS lives at Namecheap. Web records:

- `@` A records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `www` CNAME → `sevenoaksdigital.github.io`
- TXT record from the GitHub org's Pages domain verification

**Do not change the email records** (MX, SPF, DKIM, DMARC) — the domain's mailboxes are in use.
