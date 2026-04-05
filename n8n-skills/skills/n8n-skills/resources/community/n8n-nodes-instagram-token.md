# n8n-nodes-instagram-token

## Basic Information

- Package: `n8n-nodes-instagram-token`
- Category: 🔧 Utilities & Tools
- Version: 2.4.2
- Maintainer: robsonmilioli
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-instagram-token)
- Repository: [View Source](https://github.com/r-milioli/n8n-nodes-insta-accessToken)

## Description

N8N nodes for Instagram API integration with access token authentication

## Installation

```
n8n-nodes-instagram-token
```

## Nodes (2)

### Instagram

- Node Type: `n8n-nodes-instagram-token.instagram`
- Version: 1
- Requires Credentials: Yes

Send messages and interact with Instagram users via Messaging API

#### Available Operations

- **Send Audio** (`sendAudio`)
  Send an audio message
- **Send Button Template** (`sendButtonTemplate`)
  Send a message with buttons
- **Send Generic Template** (`sendGenericTemplate`)
  Send a carousel of cards
- **Send Image** (`sendImage`)
  Send an image message
- **Send Quick Replies** (`sendQuickReplies`)
  Send a message with quick reply options
- **Send Private Reply** (`sendPrivateReply`)
  Send a private reply to a comment
- **Send Private Reply (Quick Replies)** (`sendPrivateReplyQuickReplies`)
  Send a private reply with quick reply options
- **Send Text** (`sendText`)
  Send a text message
- **Send Video** (`sendVideo`)
  Send a video message
- **Upload Media** (`uploadMedia`)
  Upload media to Instagram

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `postMediaType` | options | Yes | `"IMAGE"` |
| `carouselChildren` | fixedCollection | Yes | `{}` |
| `storyMediaType` | options | Yes | `"IMAGE"` |
| `recipientId` | string | Yes | `""` |
| `messageText` | string | Yes | `""` |
| `commentId` | string | Yes | `""` |
| `messageText` | string | Yes | `""` |
| `recipientId` | string | Yes | `""` |
| `imageUrl` | string | Yes | `""` |
| `recipientId` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Instagram",
  "type": "n8n-nodes-instagram-token.instagram",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "postMediaType": "IMAGE",
    "carouselChildren": {},
    "storyMediaType": "IMAGE",
    "recipientId": "",
    "messageText": "",
    "operation": "sendAudio"
  }
}
```

---

### Instagram Trigger

- Node Type: `n8n-nodes-instagram-token.instagramTrigger`
- Version: 1
- Requires Credentials: Yes

Triggers workflow on Instagram webhook events (messages, postbacks, etc.)

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `events` | multiOptions | No | `["messages"]` |
| `ignoreEcho` | boolean | No | `true` |
| `notice` | notice | No | `""` |

#### Connection

- Input Types: 
- Output Types: `main`
- Output Count: 5

#### Example Configuration

```json
{
  "name": "Instagram Trigger",
  "type": "n8n-nodes-instagram-token.instagramTrigger",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {}
}
```

---

---

[← Back to Community Nodes Index](README.md)
