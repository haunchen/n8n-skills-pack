# n8n-nodes-zapi

## Basic Information

- Package: `n8n-nodes-zapi`
- Category: 💬 Communication & Messaging
- Version: 0.1.0
- Maintainer: leandcesar
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-zapi)
- Repository: [View Source](https://github.com/leandcesar/n8n-nodes-zapi)

## Description

Custom n8n node for Z-API.

## Installation

```
n8n-nodes-zapi
```

## Nodes (1)

### Z-API

- Node Type: `n8n-nodes-zapi.zapi`
- Version: 1
- Requires Credentials: Yes

Send messages

#### Available Operations

- **Send Audio** (`send-audio`)
  Send audio message
- **Send Document** (`send-document`)
  Send document message
- **Send GIF** (`send-gif`)
  Send GIF message
- **Send Image** (`send-image`)
  Send image message
- **Send Location** (`send-location`)
  Send location message
- **Send Options List** (`send-option-list`)
  Send text message with options list
- **Send PTV** (`send-ptv`)
  Send PTV message
- **Send Sticker** (`send-sticker`)
  Send sticker message
- **Send Text** (`send-text`)
  Send text message
- **Send Video** (`send-video`)
  Send video message

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `optionList` | fixedCollection | Yes | `{}` |
| `phone` | string | Yes | `""` |
| `text` | string | Yes | `""` |
| `optionListButtonLabel` | string | Yes | `""` |
| `optionListTitle` | string | Yes | `""` |
| `urlOrBase64` | string | Yes | `""` |
| `extension` | string | Yes | `""` |
| `resource` | options | No | `"send-message"` |
| `operation` | options | No | `"send-text"` |
| `additionalFields` | collection | No | `{}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Z-API",
  "type": "n8n-nodes-zapi.zapi",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "optionList": {},
    "phone": "",
    "text": "",
    "optionListButtonLabel": "",
    "optionListTitle": "",
    "operation": "send-audio"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
