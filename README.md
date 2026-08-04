# Tripadvisor (tripadvisor)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Tripadvisor is the world's largest travel guidance platform, helping hundreds of millions of travelers each month find places to stay, things to do, and restaurants through reviews, photos, and tools. The platform maintains over 7.5 million locations and 1 billion reviews across 43 markets and 29 languages. Tripadvisor provides APIs for content integration, hotel connectivity, and restaurant reservations.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/apis.yml)

## Tags

- Attractions
- Hotels
- Hospitality
- Restaurants
- Reviews
- Travel

## Timestamps

- **Created:** 2026-05-03
- **Modified:** 2026-06-03

## APIs

### Tripadvisor Content API

The Tripadvisor Content API provides developers with access to Tripadvisor's extensive dataset of more than 7.5 million locations, 1 billion reviews and opinions, and content in 29 languages. The API includes endpoints for location search, nearby search, location details, location photos, and location reviews, enabling developers to integrate rich travel content into their websites and applications. The first 5,000 API calls per month are free, making it accessible for initial development and testing.

- **Human URL:** [https://developer-tripadvisor.com/content-api/](https://developer-tripadvisor.com/content-api/)
- **Base URL:** `https://api.content.tripadvisor.com/api/v1`

#### Tags

- Attractions
- Hotels
- Locations
- Restaurants
- Reviews
- Travel

#### Properties

- [Documentation](https://developer-tripadvisor.com/content-api/)
- [OpenAPI](openapi/tripadvisor-content-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tripadvisor-content-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tripadvisor-content-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tripadvisor Hotel Availability Check API

The Tripadvisor Hotel Availability Check (HAC) API allows hotel booking partners to display their availability and pricing on Tripadvisor. When a user views a hotel page, Tripadvisor sends HTTP POST requests to the partner's API to retrieve real-time price and availability data. The API supports batch requests for multiple hotels and requires responses within 5 seconds on average. The current version (v8) provides richer availability data to help partners increase conversions.

- **Human URL:** [https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/](https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/)
- **Base URL:** `https://partner-endpoint.example.com`

#### Tags

- Availability
- Booking
- Connectivity
- Hospitality
- Hotels
- Travel

#### Properties

- [Documentation](https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/)
- [OpenAPI](openapi/tripadvisor-hotel-availability-check-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tripadvisor-hotel-availability-check-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tripadvisor-hotel-availability-check-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tripadvisor Hotel Inventory API

The Tripadvisor Hotel Inventory API enables connectivity partners to manage their hotel inventory listings on the Tripadvisor platform. Partners use this API to register and update the hotels they can provide availability and pricing data for, ensuring that their connected properties are accurately represented. This API works in conjunction with the Hotel Availability Check API as part of Tripadvisor's connectivity solutions for the hospitality industry.

- **Human URL:** [https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/documentation/hotel_inventory/](https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/documentation/hotel_inventory/)
- **Base URL:** `https://partner-endpoint.example.com`

#### Tags

- Connectivity
- Hospitality
- Hotels
- Inventory
- Travel

#### Properties

- [Documentation](https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/documentation/hotel_inventory/)
- [OpenAPI](openapi/tripadvisor-hotel-availability-check-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tripadvisor-hotel-availability-check-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tripadvisor-hotel-availability-check-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/tripadvisor)
- [Website](https://www.tripadvisor.com)
- [Developer Portal](https://developer-tripadvisor.com)
- [Documentation](https://tripadvisor-content-api.readme.io/reference/overview)
- [Sign Up](https://developer-tripadvisor.com/content-api/)
- [Terms of Service](https://developer-tripadvisor.com/content-api/terms-of-use/)
- [GitHub Organization](https://github.com/tripadvisor)
- [GitHub Organization](https://github.com/tripadvisor-dev)
- [JSON-LD](json-ld/tripadvisor-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/tripadvisor-location-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripadvisor-review-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripadvisor-hotel-availability-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Spectral Rules](rules/tripadvisor-rules.yml)
- [Vocabulary](vocabulary/tripadvisor-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [L L Ms Txt](https://tripadvisor-content-api.readme.io/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
