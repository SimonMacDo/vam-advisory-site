# VAM Advisory website rebuild

Staging and rebuild repository for a future VAM Advisory static website. GitHub is the source of truth. Default branch: `main`.

## Scope and boundaries

- Preserve the existing live website at https://vamadvisory.com throughout development.
- Do not change the live domain, DNS, nameservers, email records or hosting.
- Do not connect a custom domain or enable automatic deployment during initial setup.
- This repository contains structural placeholders, not an approved redesign or replacement website.
- This repository is public. Do not commit credentials, client information or unpublished personal data.

## Structure

| Path | Purpose |
| --- | --- |
| `index.html` | Home placeholder |
| `services/index.html` | Services overview placeholder |
| `team/index.html` | Team overview placeholder |
| `team/vera-tan/index.html` | Dedicated Vera Tan profile placeholder |
| `contact/index.html` | Contact placeholder |
| `assets/css/style.css` | Shared styles |
| `assets/js/` | Future scripts |
| `assets/images/` | Approved imagery |
| `assets/fonts/` | Licensed fonts |
| `robots.txt` | Development crawler block |
| `sitemap.xml` | Empty development sitemap |
| `docs/seo-plan.md` | Content, SEO and launch requirements |

## Local preview

No framework, package installation or build step is required. From the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://localhost:8000. Keep preview access local until a separate staging environment has been approved.

## Search visibility during development

`robots.txt` requests that crawlers avoid all paths. Every HTML placeholder also includes `noindex, nofollow, noarchive`.

Robots rules are voluntary, not access control. A disallowed URL can still appear in search results without its content being crawled. A crawler blocked by robots.txt cannot read the page's noindex instruction. Therefore keep staging unpublished, or protect any future preview with authentication. Public GitHub repository content may itself be indexed independently of these website rules.

Do not add staging URLs to sitemaps, submit them to search engines or point the live domain at this repository. The sitemap remains empty until production URLs and launch timing are approved.

## Planned SEO direction

Improve accurate, useful coverage of VAM Advisory, VAM Advisory Hong Kong, VAM Advisory Limited, Vera Tan, Vera Tan VAM Advisory, and verified consulting/advisory services. Give Vera her own substantive profile linked from the team page. Verify the legal entity name, services, credentials and contact details before publishing claims. See `docs/seo-plan.md`.

## Next step

Audit the existing website in read-only mode and agree the positioning, service list, page inventory and verified Vera Tan biography. Record existing URLs and prepare a redirect mapping before any later migration.

Production launch requires separate approval. Review indexing rules, approved metadata, canonical URLs, structured data, sitemap and redirects before deployment. Live infrastructure changes remain outside the initial setup scope.
