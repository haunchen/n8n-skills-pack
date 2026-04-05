# n8n-nodes-cloudinary

## Basic Information

- Package: `n8n-nodes-cloudinary`
- Category: 🔄 Data Processing
- Version: 0.0.9
- Maintainer: sveta_s
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-cloudinary)
- Repository: [View Source](https://github.com/cloudinary/n8n-nodes-cloudinary)

## Description

The official Cloudinary n8n node - upload media, update asset tags and metadata, and more

## Installation

```
n8n-nodes-cloudinary
```

## Nodes (1)

### Cloudinary

- Node Type: `n8n-nodes-cloudinary.cloudinary`
- Version: 1
- Requires Credentials: Yes

Upload to Cloudinary

#### Available Operations

- **Upload From URL** (`uploadUrl`)
  Upload an asset from URL
- **Upload File** (`uploadFile`)
  Upload an asset from file data

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `url` | string | Yes | `""` |
| `type` | options | Yes | `"upload"` |
| `getTagsResourceType` | options | Yes | `"image"` |
| `publicId` | string | Yes | `""` |
| `tags` | string | Yes | `""` |
| `structuredMetadata` | json | Yes | `"{}"` |
| `file` | string | Yes | `"data"` |
| `resource` | options | No | `"upload"` |
| `operation` | options | No | `"uploadUrl"` |
| `operation` | options | No | `"updateTags"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Cloudinary",
  "type": "n8n-nodes-cloudinary.cloudinary",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "url": "",
    "type": "upload",
    "getTagsResourceType": "image",
    "publicId": "",
    "tags": "",
    "operation": "uploadUrl"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
