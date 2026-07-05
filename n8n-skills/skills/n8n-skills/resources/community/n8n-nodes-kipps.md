# n8n-nodes-kipps

## Basic Information

- Package: `n8n-nodes-kipps`
- Category: 💬 Communication & Messaging
- Version: 1.1.0
- Maintainer: kipps.ai
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-kipps)
- Repository: [View Source](https://github.com/KIPPS-AI/n8n-nodes-kipps)

## Description

Custom Kipps.ai integration node for n8n — Chatbot, Voice Agent & WhatsApp in one node

## Installation

```
n8n-nodes-kipps
```

## Nodes (1)

### Kipps.AI

- Node Type: `n8n-nodes-kipps.kippsAi`
- Version: 1
- Requires Credentials: Yes

Interact with Kipps.AI — Chatbot, Voice Agent, or WhatsApp

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `agentId` | options | Yes | `""` |
| `message` | string | Yes | `""` |
| `voicebotId` | options | Yes | `""` |
| `phoneNumber` | string | Yes | `""` |
| `roomName` | string | Yes | `""` |
| `whatsappAgentUuid` | options | Yes | `""` |
| `to` | string | Yes | `""` |
| `templateName` | options | Yes | `""` |
| `mappedParameters` | resourceMapper | Yes | `{"mappingMode":"defineBelow","value":{}}` |
| `agentType` | options | No | `"chatbot"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Kipps.AI",
  "type": "n8n-nodes-kipps.kippsAi",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "agentId": "",
    "message": "",
    "voicebotId": "",
    "phoneNumber": "",
    "roomName": ""
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
