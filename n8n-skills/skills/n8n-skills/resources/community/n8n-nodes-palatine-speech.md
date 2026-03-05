# n8n-nodes-palatine-speech

## Basic Information

- Package: `n8n-nodes-palatine-speech`
- Category: 🤖 AI & Voice Tools
- Version: 1.0.1
- Maintainer: palatine_zealot
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-palatine-speech)
- Repository: [View Source](https://github.com/PalatineVision/n8n-nodes-palatine-speech)

## Description

Official n8n node for Palatine Speech API: transcription, diarization, sentiment analysis, summarization and more

## Installation

```
n8n-nodes-palatine-speech
```

## Nodes (1)

### Palatine Speech

- Node Type: `n8n-nodes-palatine-speech.PalatineSpeechNode`
- Version: 1
- Requires Credentials: Yes

Use Palatine Speech API to transcribe audio, diarize speakers, analyze sentiment, generate AI summaries and more

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `task` | options | No | `"transcribe"` |
| `model` | options | No | `"palatine_small"` |
| `summarizeTask` | options | No | `"meeting_summary"` |
| `binaryProperty` | string | No | `"data"` |
| `pollIntervalMs` | number | No | `500` |
| `pollIntervalMsSummarize` | number | No | `20000` |
| `maxPollAttempts` | number | No | `200` |
| `maxPollAttemptsSummarize` | number | No | `500` |
| `summarizePrompt` | string | No | `""` |
| `summarizeThinking` | boolean | No | `false` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Palatine Speech",
  "type": "n8n-nodes-palatine-speech.PalatineSpeechNode",
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
