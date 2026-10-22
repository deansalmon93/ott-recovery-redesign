# OTT Recovery redesign — SEO and testing report

22 October 2026

## Scope and result

Rebuilt the supplied breakdown assistance page as a responsive, black-and-red static website. Original business details, phone/email, service types, passenger capacity and coverage retained; long repeated copy condensed. Two new illustrative photographs were generated, including the original logo applied to the recovery truck. This is a separate review site, not a replacement already installed on ottrecoverybreakdown.ie.

## Original page audit

Source: https://www.ottrecoverybreakdown.ie/breakdown-assistance/ (live browser inspection plus public text retrieval).

- Existing title: “Breakdown Assistance 24/7 - Dublin - Meath - Kildare”. Relevant geographic targeting already exists.
- Existing description: “We offer 24 hours breakdown assistance for low prices. Our fleet offers really fast times to get to your vehicle roadside. Call 0861952598”. Rewritten for clarity, service specifics and readable contact formatting.
- A correct self-referencing canonical already exists. Preserved as the intended business-domain canonical.
- Existing Organization, WebSite and WebPage JSON-LD already exists. It uses en-US; redesigned document uses en-IE and adds factual Service coverage and 24/7 availability.
- Heading hierarchy contains “HOW WE WORK” at H3 and a footer phone number at H3. Rebuilt as one H1, section H2s and subsection H3s.
- Original photographs have generic alternative text. Replaced with descriptive alt text and explicit illustrative-image wording.
- The original page repeats some reviews and includes large amounts of testimonial text. New layout uses three short attributed excerpts, without invented ratings or review schema.
- Blue calls to action conflict with the red-and-black logo. Redesigned buttons use the requested palette and clear telephone links.
- The source states arrival “under 30 mins”. Retained as an aim in an expandable response-time explanation, with location, traffic and availability qualification rather than an unconditional guarantee.

## Amendments implemented

1. Descriptive title and meta description, English-Ireland language tag, viewport and theme colour.
2. Open Graph title/description/image/URL and large-image social card metadata.
3. Valid JSON-LD Organization, Service and WebPage graph with documented contact, coverage and service hours. No invented street address, pricing, guarantees or aggregate review rating.
4. Static, crawlable content; navigation anchors and retained links to existing service pages. Verified and corrected the About link to `/about-ott-recovery-breakdown/`.
5. Responsive WebP images: hero approximately 189 KB at 1536px and 69 KB at 800px; assistance image approximately 49 KB at 1000px and 26 KB at 600px. Explicit dimensions, eager/high-priority hero and lazy-loaded secondary image.
6. System fonts, no third-party scripts, no framework runtime or trackers required for this page.
7. Keyboard-operated ARIA tabs with arrow/Home/End support, semantic details/summary disclosures, visible focus states, skip link, reduced-motion support and mobile menu state labels.
8. Direct `tel:+353861952598` and mail links, large call buttons and a mobile fixed call bar. No fake booking or contact form.
9. Public review site deliberately uses `noindex,follow`, with the business page as canonical, to avoid introducing an indexed duplicate while the original site remains live. A public link and search indexing are separate settings.

## Browser QA performed

- Desktop at 1280px: inspected hero, typography, logo, footer and content structure; no horizontal page overflow; all images loaded; one H1; no captured browser console errors.
- Service tabs: mouse activation, keyboard ArrowRight and Home, correct selected states and corresponding panels verified.
- FAQ: passenger answer expands correctly.
- Mobile responsive viewports: 390px and 320px tested in browser frames. Found and fixed small-screen headline clipping, logo sizing and a hard edge at the hero image transition.
- Mobile menu: opens, shows links, closes on navigation and scrolls to the requested section.
- Mobile recovery tab: changes selected state and displays the correct recovery/passenger details.
- Mobile fixed call bar and vertical content flow visually inspected. Tablet layout also inspected at 768px.
- These are browser viewport checks, not physical iOS/Android device tests or a cross-browser certification.
- JavaScript syntax check passed. Local HTTP response: 200.

## Remaining production SEO work requiring original hosting/account access

This is a page-level technical and content audit, not a completed Search Console, backlink or full-domain crawl audit. No Lighthouse score or Core Web Vitals score has been invented.

Before replacing the original page:

- Deploy at the existing `/breakdown-assistance/` path and keep its canonical; update social URLs/images to the business domain.
- Remove preview `noindex` only from the final production page and remove the preview footer wording. Keep review copies noindexed.
- Check original hosting robots.txt, XML sitemap, HTTP status/redirect chains, compression, cache headers and 404 handling; these were not verified by this build.
- Update the existing domain sitemap's last-modified date for the changed page and submit/inspect the URL in Search Console.
- Run PageSpeed Insights/Lighthouse on the final business-domain deployment and inspect real-user LCP/INP/CLS in Search Console. Local layout inspection cannot establish field performance.
- Validate JSON-LD with Schema.org's validator; structured data does not guarantee rich results. LocalBusiness address data should be added only if a verified public business address is provided.
- Review Google Business Profile details, service areas, citations, ranking queries, links and conversion tracking using the relevant accounts.
- Verify actual response-time policy, passenger capacity and the continued accuracy of the original 20-year experience statement with the business before replacing production content.

## Image generation

Used the built-in image generation tool. Full-size branded truck: `ott-branded-recovery-truck.png`. Optimised website assets are included in the website ZIP.

Hero prompt: photorealistic premium roadside recovery image; modern red flatbed carrying a graphite car in an Irish rural layby at blue hour; amber beacons, damp asphalt, atmospheric countryside, charcoal/red palette and left-side negative space. Edit: preserve the scene and apply the supplied OTT Towing Services artwork as perspective-correct decals on the cab door and front panel, without the reference image's black square background.

Assistance prompt: photorealistic close-up of a recovery technician's gloved hands connecting a red battery jump-start clamp in a safe layby, dark/red workwear, Irish greenery, moody shadows, soft depth of field, no added text or logos.

## Update — full site build (22 October 2026)

- Home page now covers all services and every county (Dublin, Meath, Kildare, Wicklow, Louth, nationwide). It adds the original home page facts: quotes from €50, free scrap car removal, NCT towing, motorbike/van/caravan/off-road/boat recovery and car lockout help.
- Added 12 pages at the original URL paths: services overview, nine service pages, About and Contact. Content is taken from the original site, rewritten for clarity, with typos and duplicated text removed.
- Shared header with a Services dropdown (hover, focus and click; expands inside the mobile menu), active-page highlighting, breadcrumbs, a shared four-column footer and the mobile call bar on every page.
- All links now point inside the new site rather than the old one.
- `noindex` removed; canonicals point to the business domain; sitemap.xml added.
- QA: 616 internal links, anchors and images checked with none broken; one H1 per page; no console errors; no horizontal overflow at 1280px or 390px. Header, dropdown, mobile menu, service pages, contact and home reviews were inspected visually.
- To confirm with the business: the original About page says the company was set up 10 years ago, while other pages say over 20 years. The new site uses "over 20 years' recovery experience".
