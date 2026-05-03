# Trefle

Trefle is an open, freely accessible botanical data source and REST API for plant information covering over 400,000 plant species with taxonomy, morphology, growth requirements, and geographic distributions.

**URL:** [https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Agriculture, Botany, Open Data, Plants, Science

## Timestamps

- **Created:** 2025-02-24
- **Modified:** 2026-05-03

## APIs

### Trefle API

An open botanical REST API providing access to 400,000+ plant species with full taxonomy, morphology, growth data, and geographic distributions.

**Human URL:** [https://trefle.io/](https://trefle.io/)
**Base URL:** `https://trefle.io/api/v1`
**Auth:** Token (query parameter or Authorization header)

#### Tags

- Botany, Open Data, Plants, Science

#### Properties

- [Documentation](https://docs.trefle.io/)
- [Getting Started](https://docs.trefle.io/docs/guides/getting-started)
- [OpenAPI](openapi/trefle-openapi.yml)
- [JSONSchema - Plant](json-schema/trefle-plant-schema.json)
- [JSONSchema - Species](json-schema/trefle-species-schema.json)
- [JSONLD](json-ld/trefle-context.jsonld)
- [JSONStructure](json-structure/trefle-species-structure.json)
- [Example - Search Plants](examples/trefle-search-plants-example.json)
- [Example - Get Species](examples/trefle-get-species-example.json)
- [SpectralRuleset](rules/trefle-rules.yml)
- [NaftikoCapability](capabilities/shared/trefle-api.yaml)

## API Endpoints

| Endpoint | Description |
|----------|-------------|
| `GET /plants` | List plant species |
| `GET /plants/search?q=` | Search plants by name |
| `GET /plants/{id}` | Get plant by ID or slug |
| `GET /species` | List species with detailed data |
| `GET /species/search?q=` | Search species |
| `GET /species/{id}` | Get comprehensive species data |
| `GET /kingdoms` | List botanical kingdoms |
| `GET /subkingdoms` | List botanical subkingdoms |
| `GET /divisions` | List botanical divisions |
| `GET /families` | List plant families |
| `GET /genus` | List plant genera |
| `GET /distributions` | List geographic distribution zones |
| `GET /distributions/{id}/plants` | Get plants in a specific region |

## Naftiko Capabilities

### Workflow Capabilities

| Capability | Description | Tools |
|------------|-------------|-------|
| [Botanical Data](capabilities/botanical-data.yaml) | Plant search, species detail, taxonomy, and distribution | 9 tools |

### Shared Definitions

| Capability | Description |
|------------|-------------|
| [Trefle API](capabilities/shared/trefle-api.yaml) | Plants, species, families, genus, distributions |

## Vocabulary

- [trefle-vocabulary.yml](vocabulary/trefle-vocabulary.yml) — Domain vocabulary for botanical taxonomy, morphology, and distribution concepts

## Common Properties

- [Website](https://trefle.io/)
- [Documentation](https://docs.trefle.io/)
- [Sign Up](https://trefle.io/users/sign_in)
- [GitHub](https://github.com/treflehq)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
