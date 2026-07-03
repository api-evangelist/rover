# Rover (rover)

Rover is the world's largest online marketplace for pet care, connecting pet parents with sitters and dog walkers for boarding, house sitting, drop-in visits, doggy daycare, and dog walking. Founded in 2011 and headquartered in Seattle, Rover operated as a publicly traded company (Nasdaq: ROVR) until **Blackstone completed its acquisition of Rover Group for approximately $2.3 billion on February 27, 2024**, taking the company private and delisting the stock ($11.00/share, all-cash).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/rover/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/rover/refs/heads/main/apis.yml)

## API Access Model — No Public Developer API

As of this catalog entry (2026-07-03), **Rover does not expose a public, documented developer API and does not operate a developer portal.** This was verified through several signals:

- **No developer portal / API reference.** There is no `developer.rover.com`, no published API documentation, and no OpenAPI/reference material on rover.com or in the help center.
- **Community confirmation.** Rover's own community carries the unanswered question ["Does Rover have a public API?"](https://www.rover.com/community/question/54724/does-rover-have-a-public-api/) — no official public API is offered in response.
- **GitHub org has no public API.** The [roverdotcom GitHub organization](https://github.com/roverdotcom) publishes internal engineering tooling (Django utilities such as `django-inlinecss`, `django-prefetch-utils`, `selenium-utility-belt`, `snagsby`) but **no consumer-facing API, API client, or API documentation**.
- **Only a marketing affiliate program exists.** Rover runs an [affiliate program](https://www.postaffiliatepro.com/affiliate-program-directory/rover-com-affiliate-program/) through third-party networks (Impact, CJ/Commission Junction, Rakuten, Skimlinks, ShareASale) offering up to ~15% commission on first bookings. This is a marketing/referral program with tracking links — **not a data or booking API**.
- **Third-party access is unofficial scraping only.** Programmatic access to Rover listings today is only available via unofficial third-party web scrapers (e.g. Apify's Rover pet-sitter scrapers) and browser-automation MCP connectors. These are **not** supported or sanctioned Rover APIs and can break or violate terms at any time.

If Rover exists in a partner integration ("Rover has previously *consumed* third-party APIs such as Bandwidth's communications platform"), that is inbound integration, not an outbound public API.

Because there is no real, documented, publicly accessible API surface, this entry intentionally **does not fabricate** logical APIs (Sitters, Bookings, Services, Reviews, Pets), OpenAPI definitions, rate limits, or FinOps artifacts. It should be revisited if Rover launches a partner or developer API.

## Tags

- Pet Care
- Dog Walking
- Pet Sitting
- Marketplace
- Consumer
- No Public API
- Stub

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Pricing (Marketplace Service Fees, not API pricing)

Rover has no API pricing because it has no API. As a two-sided marketplace it monetizes through **service fees** on each booking (well-sourced, see [`plans/rover-plans-pricing.yml`](plans/rover-plans-pricing.yml)):

- **Sitters / dog walkers** pay a **~20% service fee** on most bookings (they keep ~80%); **~15%** on house sitting.
- **Pet owners** pay an **~11% booking fee**, capped at **$50**, added at checkout.
- **California** differs: a **25% marketplace fee** to providers plus an **11% booking fee** to owners.
- **UK** differs: providers keep **~85%** (95% on recurring services).

Fees vary by region, service type, and pilot programs; confirm current rates in the Rover help center.

## Common Properties

- [Website](https://www.rover.com)
- [LinkedIn](https://www.linkedin.com/company/rover-com)
- [Help Center](https://support.rover.com/hc/en-us)
- [Blog](https://www.rover.com/blog/)
- [GitHub Organization](https://github.com/roverdotcom)
- [Plans](plans/rover-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
