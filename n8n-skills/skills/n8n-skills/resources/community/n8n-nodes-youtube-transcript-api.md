# n8n-nodes-youtube-transcript-api

## Basic Information

- Package: `n8n-nodes-youtube-transcript-api`
- Category: 🔧 Utilities & Tools
- Version: 2.4.3
- Maintainer: shidoverse
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-youtube-transcript-api)
- Repository: [View Source](https://github.com/akpenou/n8n-youtube-transcript)

## Description

YouTube Transcript API Nodes for n8n

## Installation

```
n8n-nodes-youtube-transcript-api
```

## Nodes (1)

### Youtube Transcript API

- Node Type: `n8n-nodes-youtube-transcript-api.youtubeTranscriptApi`
- Version: 1

Get the transcript of a youtube video

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `youtubeURL` | string | Yes | `""` |
| `language` | string | No | `"en"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Youtube Transcript API",
  "type": "n8n-nodes-youtube-transcript-api.youtubeTranscriptApi",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "youtubeURL": ""
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
