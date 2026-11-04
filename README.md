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

