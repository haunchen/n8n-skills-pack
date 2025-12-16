# n8n-nodes-notificame-hub

## Basic Information

- Package: `n8n-nodes-notificame-hub`
- Category: 💬 Communication & Messaging
- Version: 0.3.3
- Maintainer: oriondesign
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-notificame-hub)
- Repository: [View Source](https://github.com/oriondesign2015/n8n-nodes-notificame-hub)

## Description

A NotificaMe Hub automatiza a comunicação em múltiplos canais, oferecendo soluções integradas e escaláveis.

## Installation

```
n8n-nodes-notificame-hub
```

## Nodes (1)

### NotificaMe Hub

- Node Type: `n8n-nodes-notificame-hub.notificaMeHub`
- Version: 1
- Requires Credentials: Yes

Integração com NotificaMe Hub API

#### Available Operations

- **Listar Subcontas** (`listSubaccounts`)
  Retorna uma lista das subcontas criadas
- **Definir Webhook** (`definirWebhook`)
  Define o webhook para receber eventos de um canal

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `channelId` | string | Yes | `""` |
| `recipientId` | string | Yes | `""` |
| `message` | string | Yes | `""` |
| `channelId` | string | Yes | `""` |
| `recipientId` | string | Yes | `""` |
| `audioUrl` | string | Yes | `""` |
| `channelId` | string | Yes | `""` |
| `recipientId` | string | Yes | `""` |
| `fileUrl` | string | Yes | `""` |
| `channelId` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "NotificaMe Hub",
  "type": "n8n-nodes-notificame-hub.notificaMeHub",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "channelId": "",
    "recipientId": "",
    "message": "",
    "operation": "listSubaccounts"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
