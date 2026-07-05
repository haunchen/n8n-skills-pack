# n8n-nodes-placid

## Basic Information

- Package: `n8n-nodes-placid`
- Category: 🔧 Utilities & Tools
- Version: 0.1.6
- Maintainer: placidapp
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-placid)
- Repository: [View Source](https://github.com/placidapp/n8n-nodes-placid)

## Description

n8n node to interact with Placid API for creative generation

## Installation

```
n8n-nodes-placid
```

## Nodes (1)

### Placid

- Node Type: `n8n-nodes-placid.placid`
- Version: 1
- Requires Credentials: Yes

Generate images, PDFs, and videos via Placid's API

#### Available Operations

- **Create** (`create`)
  Generate a new image from a template
- **Get** (`get`)
  Retrieve an existing image by ID
- **Delete** (`delete`)
  Delete an existing image by ID

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `pdfSources` | fixedCollection | Yes | `{}` |
| `files` | fixedCollection | Yes | `{"fileItems":[{"file":"","fileName":""}]}` |
| `template_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `imageId` | string | Yes | `""` |
| `imageId` | string | Yes | `""` |
| `template_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `urlsJson` | json | Yes | `"[]"` |
| `pdfId` | string | Yes | `""` |
| `pdfId` | string | Yes | `""` |
| `template_id` | resourceLocator | Yes | `{"mode":"list","value":""}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Placid",
  "type": "n8n-nodes-placid.placid",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "pdfSources": {},
    "files": {
      "fileItems": [
        {
          "file": "",
          "fileName": ""
        }
      ]
    },
    "template_id": {
      "mode": "list",
      "value": ""
    },
    "imageId": "",
    "operation": "create"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
