# Kinetopia — Marketing Site

The marketing website for **Kinetopia**, a one-time-purchase iOS fitness tracker that runs entirely on-device.

> The fitness tracker without the subscription.

## Live site

Deployed via Cloudflare Pages from `main`.

## Stack

- Static HTML + a single shared stylesheet (`styles.css`). No build step.
- No JavaScript runtime, no third-party fonts, no analytics. Matches the no-tracking ethos of the app.
- System serif stack for headlines (matches the iOS app's New York / serif typography).

## Files

| File | Purpose |
|---|---|
| `index.html` | Homepage |
| `support.html` | FAQ + contact |
| `privacy.html` | Privacy policy |
| `styles.css` | Shared styles |
| `robots.txt` | Search engine directives |
| `sitemap.xml` | Sitemap for search engines |

## SEO

Each page targets a specific keyword cluster and includes JSON-LD structured data:

- **Homepage**: `SoftwareApplication` schema (with `Offer` for the one-time price), `Organization`, and a homepage `FAQPage` snippet with the five most-searched questions. Targets *offline fitness tracker*, *no subscription fitness app*, *private fitness app*, *Strava alternative*.
- **Support**: full `FAQPage` schema covering all 21 Q&A pairs (eligible for Google rich snippets). Targets *Kinetopia support*, *Kinetopia FAQ*.
- **Privacy**: `BreadcrumbList` and `WebPage` schema. Targets *private fitness app data policy*.

Open Graph and Twitter card meta tags on every page. Canonical URLs on every page. `robots.txt` allows full crawl and references the sitemap.

## Editing

Open any `.html` file in a browser to preview locally. Edit, commit, push — Cloudflare Pages publishes the change within a minute.

## TODO

- [ ] Add `og.png` (1200×630) for social sharing previews. Currently referenced in meta tags but not yet present.
- [ ] Add `favicon.ico` and `apple-touch-icon.png`.

## Related

- **Caltopia** — calorie tracker sibling — <https://caltopia.org>
- Both apps are by [Cole Williams](mailto:contact@kinetopia.org).
