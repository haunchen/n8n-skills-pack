# n8n-nodes-notionmd

## Basic Information

- Package: `n8n-nodes-notionmd`
- Category: 🔄 Data Processing
- Version: 0.1.0
- Maintainer: minhlucvan
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-notionmd)
- Repository: [View Source](https://github.com/minhlucvan/n8n-nodes-notionmd)

## Description

n8n node to transform markdown to notion blocks

## Installation

```
n8n-nodes-notionmd
```

## Nodes (1)

### Notion MD

- Node Type: `n8n-nodes-notionmd.notionMd`
- Version: 1

Node to transform markdown and notion blocks

#### Available Operations

- **Markdown to Notion** (`markdownToNotion`)
- **Notion to Markdown** (`notionToMarkdown`)

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `operation` | options | No | `"markdownToNotion"` |
| `input` | string | No | `""` |
| `outputKey` | string | No | `"output"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Notion MD",
  "type": "n8n-nodes-notionmd.notionMd",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "operation": "markdownToNotion"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
