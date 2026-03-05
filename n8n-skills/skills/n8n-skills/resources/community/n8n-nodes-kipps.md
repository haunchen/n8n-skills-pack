# n8n-nodes-kipps

## Basic Information

- Package: `n8n-nodes-kipps`
- Category: 🤖 AI & Voice Tools
- Version: 0.0.12
- Maintainer: kipps.ai
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-kipps)
- Repository: [View Source](https://github.com/KIPPS-AI/n8n-nodes-kipps)

## Description

Custom Kipps.ai integration node for n8n

## Installation

```
n8n-nodes-kipps
```

## Nodes (2)

### Kipps.AI ChatAgent

- Node Type: `n8n-nodes-kipps.kippsAiChatAgent`
- Version: 1
- Requires Credentials: Yes

Interact with a Kipps.AI ChatAgent to send and receive messages.

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `agentId` | string | Yes | `""` |
| `message` | string | Yes | `""` |
| `session` | string | No | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Kipps.AI ChatAgent",
  "type": "n8n-nodes-kipps.kippsAiChatAgent",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "agentId": "",
    "message": ""
  }
}
```

---

### Kipps.AI VoiceAgent

- Node Type: `n8n-nodes-kipps.kippsAiVoiceAgent`
- Version: 1
- Requires Credentials: Yes

Manage and interact with a Kipps.AI VoiceAgent for handling calls.

#### Available Operations

- **Start Call** (`startCall`)
- **Send Audio/Text** (`sendAudioText`)
- **End Call** (`endCall`)

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `voiceagentId` | string | Yes | `""` |
| `phoneNumber` | string | Yes | `""` |
| `roomName` | string | Yes | `""` |
| `action` | options | No | `"startCall"` |
| `inputType` | options | No | `"text"` |
| `textInput` | string | No | `""` |
| `audioInput` | string | No | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Kipps.AI VoiceAgent",
  "type": "n8n-nodes-kipps.kippsAiVoiceAgent",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "voiceagentId": "",
    "phoneNumber": "",
    "roomName": "",
    "operation": "startCall"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
