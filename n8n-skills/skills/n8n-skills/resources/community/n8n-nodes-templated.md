# n8n-nodes-templated

## Basic Information

- Package: `n8n-nodes-templated`
- Category: 📄 Document Processing
- Version: 0.4.5
- Maintainer: templated.io
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-templated)
- Repository: [View Source](https://github.com/templated-io/n8n-nodes-templated)

## Description

n8n node to automate the generation of images, videos, and PDFs with Templated (https://templated.io).

## Installation

```
n8n-nodes-templated
```

## Nodes (1)

### Templated

- Node Type: `n8n-nodes-templated.templated`
- Version: 1
- Requires Credentials: Yes

Automate the generation of images, videos, and PDFs with Templated (https://templated.io)

#### Available Operations

- **Create a Render** (`createRender`)
  Generate an image, video, or PDF from a template
- **Merge Renders** (`mergeRenders`)
  Merge multiple renders into a single PDF
- **Retrieve a Render** (`retrieveRender`)
  Get details of a specific render
- **Clone a Template** (`cloneTemplate`)
  Create a clone of an existing template (maintains link to source)
- **Create a Template** (`createTemplate`)
  Create a new template programmatically with layers
- **List All Templates** (`listTemplates`)
  Get a list of all templates in your account
- **List Template Layers** (`listTemplateLayers`)
  Get all layers of a specific template
- **List Template Pages** (`listTemplatePages`)
  Get all pages of a multi-page template
- **List Template Renders** (`listTemplateRenders`)
  Get all renders created from a specific template
- **Retrieve a Template** (`retrieveTemplate`)
  Get details of a specific template
- ... and 1 more operations

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `renders` | fixedCollection | Yes | `{}` |
| `template` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `renderId` | string | Yes | `""` |
| `templateName` | string | Yes | `""` |
| `width` | number | Yes | `1200` |
| `height` | number | Yes | `630` |
| `layersJson` | json | Yes | `"[\n  {\n    \"layer\": \"text-1\",\n    \"type\": \"text\",\n    \"text\": \"Hello World\",\n    \"x\": 100,\n    \"y\": 100,\n    \"width\": 400,\n    \"height\": 50\n  }\n]"` |
| `templateId` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `templateId` | resourceLocator | Yes | `{"mode":"list","value":""}` |
| `templateId` | resourceLocator | Yes | `{"mode":"list","value":""}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Templated",
  "type": "n8n-nodes-templated.templated",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "renders": {},
    "template": {
      "mode": "list",
      "value": ""
    },
    "renderId": "",
    "templateName": "",
    "width": 1200,
    "operation": "createRender"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
