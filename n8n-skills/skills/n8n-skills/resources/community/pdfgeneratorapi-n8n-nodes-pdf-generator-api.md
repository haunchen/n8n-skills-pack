# @pdfgeneratorapi/n8n-nodes-pdf-generator-api

## Basic Information

- Package: `@pdfgeneratorapi/n8n-nodes-pdf-generator-api`
- Category: 📄 Document Processing
- Version: 0.4.0
- Maintainer: taneltahepold
- npm: [View Package](https://www.npmjs.com/package/@pdfgeneratorapi/n8n-nodes-pdf-generator-api)
- Repository: [View Source](https://github.com/pdfgeneratorapi/n8n-nodes-pdf-generator-api)

## Description

PDF Generator API Node for n8n

## Installation

```
@pdfgeneratorapi/n8n-nodes-pdf-generator-api
```

## Nodes (1)

### PDF Generator API

- Node Type: `@pdfgeneratorapi/n8n-nodes-pdf-generator-api.pdfGeneratorApi`
- Version: 1
- Requires Credentials: Yes

Generate PDFs, manage templates, convert HTML/URLs to PDF, and perform PDF operations like watermarking, encryption, and optimization

#### Available Operations

- **Generate QR Code** (`generateQRCode`)
  Generate a QR code image

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `url` | string | Yes | `""` |
| `templates` | fixedCollection | Yes | `{"templateList":[{}]}` |
| `fileUrl` | string | Yes | `""` |
| `fileBase64` | string | Yes | `""` |
| `decryptionPassword` | string | Yes | `""` |
| `formFieldsData` | json | Yes | `"{}"` |
| `publicId` | string | Yes | `""` |
| `templateId` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `templateId` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `outputId` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "PDF Generator API",
  "type": "@pdfgeneratorapi/n8n-nodes-pdf-generator-api.pdfGeneratorApi",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "url": "",
    "templates": {
      "templateList": [
        {}
      ]
    },
    "fileUrl": "",
    "fileBase64": "",
    "decryptionPassword": "",
    "operation": "generateQRCode"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
