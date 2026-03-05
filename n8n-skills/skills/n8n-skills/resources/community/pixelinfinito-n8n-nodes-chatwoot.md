# @pixelinfinito/n8n-nodes-chatwoot

## Basic Information

- Package: `@pixelinfinito/n8n-nodes-chatwoot`
- Category: 💬 Communication & Messaging
- Version: 0.3.1
- Maintainer: mctlisboa
- npm: [View Package](https://www.npmjs.com/package/@pixelinfinito/n8n-nodes-chatwoot)
- Repository: [View Source](https://github.com/pixelinfinito/n8n-nodes-chatwoot)

## Description

n8n community node for Chatwoot API integration

## Installation

```
@pixelinfinito/n8n-nodes-chatwoot
```

## Nodes (1)

### Chatwoot

- Node Type: `@pixelinfinito/n8n-nodes-chatwoot.chatwoot`
- Version: 1
- Requires Credentials: Yes

Interact with Chatwoot API

#### Available Operations

- **Get** (`get`)
  Get account details

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `url` | string | Yes | `""` |
| `status` | options | Yes | `"open"` |
| `contactId` | number | Yes | `""` |
| `conversationId` | number | Yes | `""` |
| `sourceId` | string | Yes | `""` |
| `inboxId` | number | Yes | `""` |
| `initialMessage` | string | Yes | `""` |
| `conversationId` | number | Yes | `""` |
| `messageId` | number | Yes | `""` |
| `content` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Chatwoot",
  "type": "@pixelinfinito/n8n-nodes-chatwoot.chatwoot",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "url": "",
    "status": "open",
    "contactId": "",
    "conversationId": "",
    "sourceId": "",
    "operation": "get"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
