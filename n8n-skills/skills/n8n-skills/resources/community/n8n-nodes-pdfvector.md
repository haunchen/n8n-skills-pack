# n8n-nodes-pdfvector

## Basic Information

- Package: `n8n-nodes-pdfvector`
- Category: 🤖 AI & Voice Tools
- Version: 2.0.5
- Maintainer: GitHub Actions
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-pdfvector)
- Repository: [View Source](https://github.com/phuctm97/n8n-nodes-pdfvector)

## Description

n8n community node for PDF Vector — parse PDF, Word, Excel, and image documents, extract structured data with JSON Schema, ask AI questions, and search academic papers across multiple databases.

## Installation

```
n8n-nodes-pdfvector
```

## Nodes (1)

### PDF Vector

- Node Type: `n8n-nodes-pdfvector.pdfVector`
- Version: 2
- Requires Credentials: Yes

Convert PDFs, Word, Excel documents, and images to clean markdown, extract structured data with AI, process invoices with specialized parsing, and search millions of academic papers across PubMed, ArXiv, Google Scholar, and more.

#### Available Operations

- **Parse** (`parse`)
  Extract text and page count from a document
- **Ask** (`ask`)
  Ask a question about a document and get an AI answer
- **Extract** (`extract`)
  Extract structured data from a document using JSON Schema

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `query` | string | Yes | `""` |
| `binaryPropertyName` | string | Yes | `"data"` |
| `question` | string | Yes | `""` |
| `prompt` | string | Yes | `""` |
| `schema` | json | Yes | `"{\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": { \"type\": \"string\" },\n    \"summary\": { \"type\": \"string\" }\n  },\n  \"required\": [\"title\"]\n}"` |
| `binaryPropertyName` | string | Yes | `"data"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "PDF Vector",
  "type": "n8n-nodes-pdfvector.pdfVector",
  "typeVersion": 2,
  "position": [
    250,
    300
  ],
  "parameters": {
    "url": "",
    "query": "",
    "operation": "parse"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
