# n8n-nodes-docx-converter

## Basic Information

- Package: `n8n-nodes-docx-converter`
- Category: 📄 Document Processing
- Version: 0.1.3
- Maintainer: cre8tiv
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-docx-converter)
- Repository: [View Source](https://github.com/cre8tiv/n8n-docx-converter)

## Description

A node to convert Docx to Text

## Installation

```
n8n-nodes-docx-converter
```

## Nodes (1)

### DOCX to Text

- Node Type: `n8n-nodes-docx-converter.docxToText`
- Version: 1

Converts DOCX file to plain text

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `inputBinaryField` | string | Yes | `"data"` |
| `destinationOutputField` | string | Yes | `"text"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "DOCX to Text",
  "type": "n8n-nodes-docx-converter.docxToText",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "inputBinaryField": "data",
    "destinationOutputField": "text"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
