# DailyClaimIt SEO setup and homepage plan

## What is available in this repository

The `main` branch contains a makeup landing page. `CNAME` points to `makeup.dailyclaimit.com`. There is no separate surveys/offer-directory homepage in this checkout. Live delivery, redirects, DNS, Google indexing, and Search Console access have not been verified from this environment.

The SEO draft adds a descriptive title and meta description, a canonical URL, social sharing metadata, WebSite/WebPage JSON-LD, sponsored affiliate-link annotations, an HTML guide linked from the landing page, `robots.txt`, and a sitemap. Existing affiliate destinations and the custom domain stay as they are. Existing `noindex` directives on privacy, terms, and the thank-you page stay in place; these pages are deliberately omitted from the sitemap but remain crawlable.

This is a draft for review, not a verified live deployment. Before merging, confirm the makeup offer is still active and update its visible claims against the new provider's terms. The legacy page simulates location, inventory, and eligibility checks with timers; those checks are not provider verification. The SEO additions do not authenticate availability or eligibility. The existing copy also makes claims about kit contents, shipping, and third-party data handling that need to match the replacement offer.

## Main-site structure to build once its hosting and offers are confirmed

Keep the makeup campaign subdomain. Build the general offer directory on `https://dailyclaimit.com/` with dedicated pages for distinct visitor needs. Proposed paths below are planning targets, not pages created by this draft.

| Proposed URL | Search topic to evaluate | What the page should help visitors do |
| --- | --- | --- |
| `/` | Surveys, samples, and sweepstakes | Choose the right category and see active offers |
| `/surveys/` | Surveys for rewards | Compare eligibility, payout type, withdrawal threshold, and estimated effort |
| `/free-samples/` | Free samples by mail | Distinguish samples from prize entries and check delivery conditions |
| `/sweepstakes/` | Sweepstakes to enter | Check the sponsor, official rules, location, and entry deadline |
| `/makeup-testing/` | Makeup product testing | Understand the offer type and reach the relevant makeup promotion |
| `/guides/surveys-vs-sweepstakes/` | Survey rewards versus prize entries | Understand whether completion earns a reward or only enters a drawing |

These are topic hypotheses. No search-volume estimates, competition scores, or ranking forecasts have been measured. Validate phrasing with actual Search Console queries and keyword research after the site is available.

For each active offer, publish verified provider details, countries/ages, reward type, requirements, any costs, and an honest last-checked date. Only describe earnings, payout methods, payment thresholds, or kit contents when the provider supports them. Add the official terms link and an affiliate disclosure. Mark expired offers clearly and update internal links. Keep useful guides at stable URLs when campaigns rotate.

## Search Console setup after deployment

1. Open https://search.google.com/search-console and add a Domain property for `dailyclaimit.com` (no protocol or path). This covers its subdomains too.
2. Use Google's actual DNS verification record at the domain's DNS provider. Do not invent a verification code or overwrite existing domain-routing records.
3. Confirm the new files are live. Submit `https://makeup.dailyclaimit.com/sitemap.xml` in the verified property. When the separate main-site sitemap exists, submit that URL too.
4. Inspect the landing-page and guide URLs with URL Inspection, check Google's rendered page and selected canonical, and request indexing if available. A submitted sitemap or indexing request does not guarantee inclusion or ranking.
5. Review impressions, clicks, search phrases, and page indexing. Use a page filter for the makeup subdomain. Check errors and actual user experience before adding more pages.

Search Console verification requires access to the owner's Google account and DNS settings; it has not been completed by this draft. GitHub repository access alone cannot verify a Search Console property.

## Measurement and upkeep

Keep paid traffic running separately from the SEO work. Track landing-page visits, offer clicks, and confirmed network conversions; a click or a visit to the thank-you page is not proof of a payable conversion. Before an organic campaign, confirm the affiliate network's approved traffic sources and sub-ID conventions so traffic-source reporting does not mistakenly label organic visitors as PropellerAds.

Start with a few useful category pages and offer comparisons. Review offer availability regularly, improve pages that receive search impressions, and link related guides to the relevant category. SEO is an ongoing publishing and maintenance task; technical tags alone do not guarantee traffic.

## Primary references

- Google SEO starter guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Added value on affiliate sites: https://developers.google.com/search/docs/essentials/spam-policies#thin-affiliation
- Canonical URLs: https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls
- Sitemaps: https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap
- Sponsored links: https://developers.google.com/search/docs/crawling-indexing/qualify-outbound-links
- Search Console properties: https://support.google.com/webmasters/answer/34592
- Crawlable noindex pages: https://developers.google.com/search/docs/crawling-indexing/block-indexing
