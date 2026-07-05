# n8n-nodes-businessmap

## Basic Information

- Package: `n8n-nodes-businessmap`
- Category: 🔧 Utilities & Tools
- Version: 1.1.1
- Maintainer: GitHub Actions
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-businessmap)
- Repository: [View Source](https://github.com/kanbanize/n8n-nodes-businessmap)

## Description

An n8n community node package that integrates with Businessmap's REST API for CRUD operations on boards, cards and workflow artifacts across enterprise environments.

## Installation

```
n8n-nodes-businessmap
```

## Nodes (2)

### Businessmap

- Node Type: `n8n-nodes-businessmap.businessmap`
- Version: 1
- Requires Credentials: Yes

Use Businessmap API v2

#### Available Operations

- **Create** (`create`)
  Create card
- **Update** (`update`)
  Update card
- **Move** (`move`)
  Move card
- **Get Card** (`get`)
  Get card by ID
- **Get Custom Card** (`getCustom`)
  Get card by custom card ID
- **Get All Cards Per Board** (`getAllCardsPerBoard`)
  Retrieve all cards from a board

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `output` | options | Yes | `"simplified"` |
| `output_fields` | multiOptions | Yes | `["card_id"]` |
| `output` | options | Yes | `"simplified"` |
| `output_fields` | multiOptions | Yes | `["card_id"]` |
| `link_type` | options | Yes | `"relatives"` |
| `link_type` | options | Yes | `"relatives"` |
| `time_unit` | options | Yes | `"hours"` |
| `board_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `workflow_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `lane_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Businessmap",
  "type": "n8n-nodes-businessmap.businessmap",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "output": "simplified",
    "output_fields": [
      "card_id"
    ],
    "link_type": "relatives",
    "operation": "create"
  }
}
```

---

### Businessmap Trigger

- Node Type: `n8n-nodes-businessmap.businessmapTrigger`
- Version: 1
- Requires Credentials: Yes

Starts the workflow when Businessmap events occur

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `events` | multiOptions | Yes | `[]` |
| `board_id` | options | Yes | `""` |
| `authenticate_webhook` | boolean | No | `true` |

#### Connection

- Input Types: 
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Businessmap Trigger",
  "type": "n8n-nodes-businessmap.businessmapTrigger",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "events": [],
    "board_id": ""
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
