# gitforce.net — GitForce project site

The landing page for **GitForce** — a byte-compatible implementation of Git written
in Apex, running on Salesforce. Served via GitHub Pages at
**[gitforce.net](https://gitforce.net)**.

This repo contains only the static site (a single `index.html`, no build step). The
GitForce source code lives in a separate repository.

## Hosting

- Static HTML, served by GitHub Pages from the default branch root.
- `CNAME` binds the custom domain `gitforce.net`.
- `.nojekyll` disables Jekyll processing (plain HTML, nothing to build).

## DNS (for the custom domain)

Point `gitforce.net` at GitHub Pages:

| Type  | Name | Value |
|-------|------|-------|
| A     | `@`  | `185.199.108.153` |
| A     | `@`  | `185.199.109.153` |
| A     | `@`  | `185.199.110.153` |
| A     | `@`  | `185.199.111.153` |
| CNAME | `www` | `<org>.github.io.` |

Then in the repo: **Settings → Pages → Custom domain → `gitforce.net`**, and enable
**Enforce HTTPS** once the certificate is issued.

## License

MIT © 2026 Dustin Kost. GitForce is an independent project, not affiliated with or
endorsed by Git, GitHub, or Salesforce.
