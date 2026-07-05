# @searchapi/n8n-nodes-searchapi

## Basic Information

- Package: `@searchapi/n8n-nodes-searchapi`
- Category: 🕷️ Web Scraping & Browser Automation
- Version: 2.0.4
- Maintainer: searchapi_team
- npm: [View Package](https://www.npmjs.com/package/@searchapi/n8n-nodes-searchapi)
- Repository: [View Source](https://github.com/SearchApi/n8n-nodes-searchapi)

## Description

SearchApi.io nodes for n8n

## Installation

```
@searchapi/n8n-nodes-searchapi
```

## Nodes (1)

### SearchApi

- Node Type: `@searchapi/n8n-nodes-searchapi.searchApi`
- Version: 1
- Requires Credentials: Yes

Access real-time search results from Google, Google Images, Google Maps, Google Shopping and more. Use this when you need current, up-to-date information, product searches, location data, or visual content that may not be available in your training data.

#### Available Operations

- **Search** (`search`)
  Search using the engine specified in the resource

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `q` | string | Yes | `""` |
| `q` | string | Yes | `""` |
| `q` | string | Yes | `""` |
| `q` | string | Yes | `""` |
| `resource` | options | No | `"google"` |
| `operation` | options | No | `"search"` |
| `locationSettings` | collection | No | `{}` |
| `languageSettings` | collection | No | `{}` |
| `searchOptions` | collection | No | `{}` |
| `timeFilters` | collection | No | `{}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "SearchApi",
  "type": "@searchapi/n8n-nodes-searchapi.searchApi",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "q": "",
    "operation": "search"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
