# n8n-nodes-autype

## Basic Information

- Package: `n8n-nodes-autype`
- Category: 📄 Document Processing
- Version: 1.0.5
- Maintainer: centerbit_co
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-autype)
- Repository: [View Source](https://github.com/centerbitco/n8n-nodes-autype)

## Description

n8n community node for the Autype Developer API — document generation, PDF tools, bulk rendering, and more.

## Installation

```
n8n-nodes-autype
```

## Nodes (1)

### Autype

- Node Type: `n8n-nodes-autype.autype`
- Version: 1
- Requires Credentials: Yes

Interact with the Autype Developer API for document generation, PDF tools, and more

#### Available Operations

- **Download Output** (`download`)
  Download the rendered document file by job ID
- **Get Job Status** (`getStatus`)
  Get the current status of a render job
- **List Jobs** (`list`)
  List all render jobs for the organization
- **Render From JSON** (`renderJson`)
  Submit document JSON for rendering to PDF, DOCX, or ODT
- **Render From Markdown** (`renderMarkdown`)
  Submit Extended Markdown content for rendering
- **Render Persistent Document** (`renderDocument`)
  Render a pre-existing document from your workspace by ID
- **Validate JSON** (`validateJson`)
  Validate a document JSON without rendering (no credits charged)
- **Validate Markdown** (`validateMarkdown`)
  Validate Extended Markdown content without rendering (no credits charged)

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `format` | options | Yes | `"PDF"` |
| `angle` | options | Yes | `90` |
| `mode` | options | Yes | `"keep"` |
| `config` | json | Yes | `"{\n  \"document\": { \"type\": \"pdf\", \"size\": \"A4\" },\n  \"sections\": [\n    {\n      \"type\": \"flow\",\n      \"content\": [\n        { \"type\": \"h1\", \"text\": \"Hello World\" },\n        { \"type\": \"text\", \"text\": \"This is a paragraph.\" }\n      ]\n    }\n  ]\n}"` |
| `content` | string | Yes | `""` |
| `documentId` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `documentId` | string | Yes | `""` |
| `items` | json | Yes | `"[{\"name\": \"Acme Inc\", \"date\": \"2024-01-01\"}]"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Autype",
  "type": "n8n-nodes-autype.autype",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "format": "PDF",
    "angle": 90,
    "mode": "keep",
    "config": "{\n  \"document\": { \"type\": \"pdf\", \"size\": \"A4\" },\n  \"sections\": [\n    {\n      \"type\": \"flow\",\n      \"content\": [\n        { \"type\": \"h1\", \"text\": \"Hello World\" },\n        { \"type\": \"text\", \"text\": \"This is a paragraph.\" }\n      ]\n    }\n  ]\n}",
    "content": "",
    "operation": "download"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
