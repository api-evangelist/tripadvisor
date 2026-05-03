# Tripadvisor

Tripadvisor is the world's largest travel guidance platform, helping hundreds of millions of travelers each month find places to stay, things to do, and restaurants through reviews, photos, and tools. The platform maintains over 7.5 million locations and 1 billion reviews across 43 markets and 29 languages. Tripadvisor provides APIs for content integration, hotel connectivity, and restaurant reservations.

**URL:** https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/apis.yml

## Tags

Attractions, Hotels, Hospitality, Restaurants, Reviews, Travel

## APIs

### Tripadvisor Content API

Provides access to Tripadvisor's dataset of 7.5M+ locations, 1B+ reviews, photos, and content in 29 languages. Includes endpoints for location search, nearby search, location details, photos, and reviews. First 5,000 calls/month free.

**Human URL:** https://developer-tripadvisor.com/content-api/  
**Base URL:** https://api.content.tripadvisor.com/api/v1

#### Properties

| Type | URL |
|------|-----|
| Documentation | https://developer-tripadvisor.com/content-api/ |
| OpenAPI | [openapi/tripadvisor-content-api-openapi.yml](openapi/tripadvisor-content-api-openapi.yml) |

#### Tags

Attractions, Hotels, Locations, Restaurants, Reviews, Travel

### Tripadvisor Hotel Availability Check API

Partner-side API that Tripadvisor queries in real-time to retrieve hotel pricing and availability for display on hotel pages. Partners implement this endpoint on their servers. Version 8.

**Human URL:** https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/

#### Properties

| Type | URL |
|------|-----|
| Documentation | https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/ |
| OpenAPI | [openapi/tripadvisor-hotel-availability-check-api-openapi.yml](openapi/tripadvisor-hotel-availability-check-api-openapi.yml) |

#### Tags

Availability, Booking, Connectivity, Hotels, Travel

### Tripadvisor Hotel Inventory API

Partner API for registering and managing hotel listings that a connectivity partner can provide availability data for.

**Human URL:** https://developer-tripadvisor.com/connectivity-solutions/hotel-availability-check-api/documentation/hotel_inventory/

## Artifacts

| Artifact | Path |
|----------|------|
| Content API OpenAPI | [openapi/tripadvisor-content-api-openapi.yml](openapi/tripadvisor-content-api-openapi.yml) |
| Hotel Availability OpenAPI | [openapi/tripadvisor-hotel-availability-check-api-openapi.yml](openapi/tripadvisor-hotel-availability-check-api-openapi.yml) |
| Location JSON Schema | [json-schema/tripadvisor-location-schema.json](json-schema/tripadvisor-location-schema.json) |
| Review JSON Schema | [json-schema/tripadvisor-review-schema.json](json-schema/tripadvisor-review-schema.json) |
| Hotel Availability JSON Schema | [json-schema/tripadvisor-hotel-availability-schema.json](json-schema/tripadvisor-hotel-availability-schema.json) |
| JSON Structure | [json-structure/tripadvisor-location-structure.json](json-structure/tripadvisor-location-structure.json) |
| JSON-LD Context | [json-ld/tripadvisor-context.jsonld](json-ld/tripadvisor-context.jsonld) |
| Spectral Rules | [rules/tripadvisor-rules.yml](rules/tripadvisor-rules.yml) |
| Vocabulary | [vocabulary/tripadvisor-vocabulary.yml](vocabulary/tripadvisor-vocabulary.yml) |

## Examples

| Example | Path |
|---------|------|
| Search for Locations | [examples/tripadvisor-search-for-locations-example.json](examples/tripadvisor-search-for-locations-example.json) |
| Get Location Details | [examples/tripadvisor-get-location-details-example.json](examples/tripadvisor-get-location-details-example.json) |
| Get Location Reviews | [examples/tripadvisor-get-location-reviews-example.json](examples/tripadvisor-get-location-reviews-example.json) |
| Check Hotel Availability | [examples/tripadvisor-check-hotel-availability-example.json](examples/tripadvisor-check-hotel-availability-example.json) |

## Capabilities

| Capability | Description |
|-----------|-------------|
| [travel-content](capabilities/travel-content.yaml) | Travel content discovery: search locations, get details, photos, and reviews |
| [hotel-connectivity](capabilities/hotel-connectivity.yaml) | Hotel connectivity partner workflow: availability check and inventory management |

### Shared Definitions

| Shared Definition | API |
|-------------------|-----|
| [content-api](capabilities/shared/content-api.yaml) | Tripadvisor Content API |
| [hotel-availability-api](capabilities/shared/hotel-availability-api.yaml) | Tripadvisor Hotel Availability Check API |

## Common Properties

- [Website](https://www.tripadvisor.com)
- [Developer Portal](https://developer-tripadvisor.com)
- [Content API Reference](https://tripadvisor-content-api.readme.io/reference/overview)
- [GitHub Organization](https://github.com/tripadvisor)
- [GitHub Developers](https://github.com/tripadvisor-dev)
- [Privacy Policy](https://www.tripadvisor.com/pages/privacy.html)
- [Terms of Service](https://www.tripadvisor.com/pages/terms.html)
- [Blog](https://www.tripadvisor.com/blog/)
- [Support](https://developer-tripadvisor.com/support/)

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
