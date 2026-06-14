# TripAdvisor GraphQL Schema

## Overview

This conceptual GraphQL schema models the TripAdvisor travel reviews and search platform. While TripAdvisor exposes a REST-based Content API, this schema captures the full domain model including locations, hotels, restaurants, attractions, reviews, photos, geographic data, and travel insights.

The schema is derived from the Tripadvisor Content API (https://tripadvisor-content-api.readme.io/reference/overview), which provides access to over 7.5 million locations, 1 billion reviews, and content across 43 markets in 29 languages.

## Root Types

### Query

- `location(locationId: ID!)` — Fetch full details for a single location by Tripadvisor location ID.
- `locationSearch(query: String!, language: String, currency: String)` — Search locations by name or keyword.
- `nearbySearch(latLong: String!, category: String, language: String)` — Find locations near a geographic coordinate.
- `locationPhotos(locationId: ID!, language: String, limit: Int, offset: Int)` — Retrieve photos for a location.
- `locationReviews(locationId: ID!, language: String, limit: Int, offset: Int)` — Retrieve traveler reviews for a location.
- `hotel(locationId: ID!)` — Fetch hotel-specific details including amenities, room types, and pricing.
- `restaurant(locationId: ID!)` — Fetch restaurant-specific details including cuisine, hours, and price level.
- `attraction(locationId: ID!)` — Fetch attraction-specific details including category and subcategory info.
- `travelInsights(locationId: ID!, travelerType: TravelerType)` — Retrieve seasonal trends and travel patterns.

## Core Domain Types

### Location Types

- `Location` — Base type for any Tripadvisor location entity (hotel, restaurant, attraction, etc.).
- `LocationDetails` — Extended details for a location including descriptions and amenities.
- `LocationSummary` — Lightweight version of a location for list and search results.
- `LocationGeo` — Geographic data associated with a location.
- `LocationDetails` — Full location payload including all nested data.

### Hospitality Types

- `Hotel` — Hotel property with rooms, amenities, pricing, and availability metadata.
- `Restaurant` — Restaurant with cuisine types, price level, hours, and reservation details.
- `Attraction` — Tourist attraction with category, admission details, and visiting hours.
- `Airline` — Airline entity with routes, ratings, and traveler reviews.
- `Cruise` — Cruise line or ship with itineraries and onboard amenities.
- `Vacation` — Vacation rental property with features and host details.

### Search Types

- `SearchResult` — A single item returned from location or nearby searches.
- `NearbySearch` — Parameters and results for geographic proximity searches.

### Media Types

- `Photo` — Individual photo with attribution, caption, and sizing.
- `PhotoAlbum` — Grouped collection of photos for a location.

### Review Types

- `Review` — A single traveler review including text, rating, and metadata.
- `ReviewScore` — Aggregate score data for a location.
- `ReviewRating` — Individual dimension ratings (cleanliness, service, value, etc.).
- `ReviewAuthor` — Profile of the traveler who wrote the review.
- `ReviewResponse` — Owner or staff response to a review.
- `OwnerResponse` — Specific response type for property owners replying to reviews.

### Rating Types

- `Rating` — Overall aggregate rating for a location.
- `RatingBreakdown` — Breakdown of ratings by score bucket (e.g., count of 5-star reviews).

### Classification Types

- `Category` — Top-level content category (Hotels, Restaurants, Attractions, etc.).
- `Subcategory` — Finer-grained classification within a category.
- `Tag` — User-generated or system-assigned tag for a location.
- `Amenity` — A specific amenity offered by a hotel or attraction.
- `Cuisine` — Cuisine type offered by a restaurant.

### Pricing Types

- `PriceLevel` — Symbolic price tier (e.g., $, $$, $$$).
- `PriceRange` — Minimum and maximum price range with currency.

### Recognition Types

- `Award` — Industry or Tripadvisor award received by a location.
- `Certificate` — Certificate of Excellence or similar recognition.
- `Accreditation` — Third-party accreditation or certification.

### Hours and Status Types

- `Hours` — Operating hours schedule for a location.
- `Period` — A single open/close period within a day.
- `OpenStatus` — Current open/closed status with next open time.

### Geographic Types

- `GeoPoint` — Latitude and longitude coordinate.
- `BoundingBox` — Geographic bounding box defined by two corners.
- `Address` — Structured postal address.
- `AddressComponent` — Individual component of a structured address.
- `Neighborhood` — Named neighborhood or district.
- `Area` — Broader geographic area or region.

### Localization Types

- `Language` — Supported language with code and display name.
- `Currency` — Currency with code, symbol, and exchange metadata.

### Travel Intelligence Types

- `TravelInfo` — General travel information for a destination.
- `TravelerType` — Enum for traveler segments (families, couples, solo, business).
- `TravelInsight` — Derived insights about traveler behavior at a location.
- `TravelDate` — Date range used for travel-specific queries.
- `SeasonalTrend` — Popularity and pricing trends by season or month.

### Community Types

- `ForumPost` — A post in the Tripadvisor travel forums.
- `TopicThread` — A forum discussion thread.
- `InfluencerMeta` — Metadata about high-contribution reviewers.

### Ranking Types

- `Popularity` — Popularity score and ranking within a category.
- `Ranking` — Position of a location within a geographic area and category.

## Usage Notes

This schema is designed to complement the TripAdvisor REST Content API. A GraphQL layer over the Content API would allow callers to request precisely the fields they need — for example, fetching a hotel with its reviews, photos, and nearby restaurants in a single query rather than multiple REST round-trips.

The types mirror the data structures documented in the Content API reference at https://tripadvisor-content-api.readme.io/reference/overview.
