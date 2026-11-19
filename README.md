# sevenoaks.digital

The company website for Seven Oaks Digital, L.L.C.: a small static site served by GitHub Pages at <https://sevenoaks.digital>.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Home page. |
| `about/index.html` | About the company. |
| `lexsum/index.html` | Short LEXSUM page that links to <https://lexsum.app>. |
| `contact/index.html` | Email, phone and mailing address. |
| `privacy/index.html` | Privacy policy for this website. |
| `404.html` | Page GitHub Pages shows for unknown URLs. |
| `site.css` | Shared styles for every page. |
| `treeline.svg` | Oak treeline at the bottom of each page header. |
| `favicon.svg` | Oak favicon, also used as the logo in the header. |
| `CNAME` | Tells GitHub Pages to serve the site at `sevenoaks.digital`. |
| `.nojekyll` | Serve files as-is (skip Jekyll processing). |

There is no build step. The header menu and footer are repeated in each page, so a change to either must be made in all six HTML files.

## Rules

- No cookies, analytics, tracking, forms, or third-party requests (fonts, CDNs, scripts). This keeps the site free of any need for a cookie banner.
- Company details (legal name "Seven Oaks Digital, L.L.C.", address and phone) must match the D-U-N-S record exactly.
- Public email addresses are `hello@sevenoaks.digital` and `support@sevenoaks.digital` only.
- Must stay responsive at 375 px, support light and dark mode via `prefers-color-scheme`, and meet WCAG AA contrast.
- Links between pages use root paths such as `/about/`, so preview from the repo root.

## Preview locally

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.
