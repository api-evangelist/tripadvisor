# Tripadvisor

Tripadvisor is the world's largest travel guidance platform, helping hundreds of millions of travelers each month find places to stay, things to do, and restaurants through reviews, photos, and tools. The platform maintains over 7.5 million locations and 1 billion reviews across 43 markets and 29 languages. Tripadvisor provides APIs for content integration, hotel connectivity, and restaurant reservations.

**URL:** https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/apis.yml

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

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

Self-contained Naftiko capabilities, one per business surface (OpenAPI tag). Each file inlines its own consumes block plus REST and MCP exposers.

### Tripadvisor Content API

| Capability | Tools | Description |
|-----------|-------|-------------|
| [content-api-location-search](capabilities/content-api-location-search.yaml) | 2 | Search locations by query and search nearby by coordinate |
| [content-api-location-details](capabilities/content-api-location-details.yaml) | 1 | Get comprehensive details for a location |
| [content-api-location-photos](capabilities/content-api-location-photos.yaml) | 1 | Get up to 5 recent photos for a location |
| [content-api-location-reviews](capabilities/content-api-location-reviews.yaml) | 1 | Get up to 5 recent reviews for a location |

### Tripadvisor Hotel Availability Check API

| Capability | Tools | Description |
|-----------|-------|-------------|
| [hotel-availability-check-api-availability](capabilities/hotel-availability-check-api-availability.yaml) | 1 | Real-time price and availability for one-to-many hotels |
| [hotel-availability-check-api-configuration](capabilities/hotel-availability-check-api-configuration.yaml) | 1 | Partner configuration discovery |

### Tripadvisor Hotel Inventory API

| Capability | Tools | Description |
|-----------|-------|-------------|
| [hotel-availability-check-api-hotel-inventory](capabilities/hotel-availability-check-api-hotel-inventory.yaml) | 1 | Daily pull of the partner's connected hotel inventory |

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
