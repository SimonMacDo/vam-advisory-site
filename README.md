# VAM Advisory website rebuild

GitHub is the source of truth for this static website. Default branch: `main`.

## Status

First review draft based on the supplied **VAM capability 2026** presentation and the instruction to lead with in-house legal documentation and litigation support. US listing services are excluded. Historical professional roles appear only as background on Vera Tan's profile.

This is a staging/rebuild repository. The existing live website at https://vamadvisory.com remains unchanged. Do not change its DNS, nameservers, email records or hosting, or connect a custom domain, without separate approval.

## Pages

- `index.html`: Home
- `services/index.html`: six service areas, with legal documentation and litigation support first
- `case-studies/index.html`: four anonymised engagements from the presentation
- `team/index.html`: team introduction
- `team/vera-tan/index.html`: dedicated founder profile
- `contact/index.html`: contact details from the presentation
- `assets/css/style.css`: responsive shared styling
- `assets/images/`: original logo and Vera photograph extracted from the supplied presentation
- `assets/js/`, `assets/fonts/`: reserved folders
- `robots.txt`, `sitemap.xml`: staging SEO files
- `docs/seo-plan.md`: SEO direction and launch requirements

## Preview and indexing

A separate GitHub Pages preview may be enabled for this repository, with no custom domain. Its purpose is review only, not replacement of the live website. GitHub Pages should publish from the root of `main`.

Every HTML page contains `noindex, nofollow, noarchive`. `robots.txt` disallows all crawling and sitemap.xml deliberately contains no URLs. Robots directives are voluntary and do not provide access control. Because robots.txt blocks crawling, crawlers may not see page-level noindex, and a publicly linked staging URL may still appear in results. The public GitHub repository may itself be indexed. Do not submit staging to search engines. If strict exclusion is required, use an authenticated preview.

## Editing and local preview

Plain HTML and CSS. No build step, dependencies, tracking scripts or form backend. Contact links open the visitor's email or phone application.

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://localhost:8000. Use relative asset and page links so the site works under the GitHub Pages repository path.

## Content review before launch

Vera should confirm service scope, biography, historic roles, the office contact details and case-study wording and figures. Client names and logos have not been published. No litigation case study, testimonial or additional outcome has been invented. Add further material when available.

Before any separately approved production launch, audit existing URLs and redirects, confirm production canonical URLs and structured data, generate the production sitemap and replace development indexing controls. Keep staging excluded from search after launch.
