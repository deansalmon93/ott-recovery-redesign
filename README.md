# OTT Recovery redesign

Responsive static website for OTT Recovery Breakdown: the redesigned home page plus every page from the original site, all sharing the same header, navigation, footer, colours and typography.

## Pages

| Path | Page |
|---|---|
| `/` | Home |
| `/breakdown-services/` | All services |
| `/commercial-vehicle-transport/` | For business: dock collections, dealer transfers, multi-car transport |
| `/breakdown-assistance/` | Breakdown assistance |
| `/breakdown-recovery/` | Breakdown recovery |
| `/towing/` | Towing service |
| `/tow-truck/` | Tow truck |
| `/accident-recovery/` | Accident recovery |
| `/car-jump-start/` | Car jump start |
| `/battery-replacement/` | Battery replacement |
| `/flat-tyre-change/` | Flat tyre change |
| `/wrong-fuel-replacement/` | Wrong fuel replacement |
| `/about-ott-recovery-breakdown/` | About |
| `/contact/` | Contact and quote request |

Every page is a single file at the top level (e.g. `towing.html`), so the site can be uploaded to GitHub without folders. Canonical tags still point to the original page addresses on www.ottrecoverybreakdown.ie.

## Run locally

Serve this folder with any static server, e.g. `python -m http.server 8000`, then open http://localhost:8000. Opening the files directly by double-clicking won't follow the folder links — use a server.

No build step is required to host the site. All pages share `style.css` and `app.js`.

## Editing

The header, menu and footer are repeated in each page's HTML. If you change one, change it on every page (search and replace across the folder works well).

## Contact form

The quote forms on `/contact/` and `/commercial-vehicle-transport/` open a pre-filled email to info@ottrecoverybreakdown.ie in the visitor's email app. It has no server and stores nothing.

## SEO

- Each page has its own title, description, canonical URL (on www.ottrecoverybreakdown.ie), Open Graph tags and JSON-LD (Organization, Service, Breadcrumb, FAQ).
- `sitemap.xml` lists every page; `robots.txt` points to it.
- Pages are indexable. If you host a preview copy elsewhere, the canonical tags point Google at the main domain.
- See SEO-and-testing-report.md for launch checks.

## Assets

The OTT logo belongs to its owner (`logo.png` is a transparent version of `logo.jpg`). The `fleet-*.webp` photos are real OTT vehicles. The red truck (`truck-*.webp`) and battery (`assistance-*.webp`) images are AI-created illustrations.
