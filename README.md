# Community Calendar Connect

The parent landing page for [communitycalendarconnect.com](https://communitycalendarconnect.com/)
— explains the product, lists which counties are live, and points
officials/newspapers/new counties toward getting their own instance.

This is not any single county's calendar. The Linn County deployment lives
in its own repo (`linn-county-calendar`), served at
[linn.communitycalendarconnect.com](https://linn.communitycalendarconnect.com/).
Each new county gets its own subdomain and its own repo the same way.

## Structure

Static site under `docs/`, served by GitHub Pages:

- `docs/index.html` — the whole page (no build step, no dependencies)
- `docs/CNAME` — GitHub Pages custom domain config, points at
  `communitycalendarconnect.com`

## Deploying

Push to `main` and GitHub Pages picks it up automatically. DNS for
`communitycalendarconnect.com` needs 4 `A` records pointing at GitHub
Pages' IPs (185.199.108.153, .109.153, .110.153, .111.153) — set at
whichever provider hosts the domain's DNS.
