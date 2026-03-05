# @gotohuman/n8n-nodes-gotohuman

## Basic Information

- Package: `@gotohuman/n8n-nodes-gotohuman`
- Category: 🤖 AI & Voice Tools
- Version: 0.1.1
- Maintainer: gotohuman-admin
- npm: [View Package](https://www.npmjs.com/package/@gotohuman/n8n-nodes-gotohuman)
- Repository: [View Source](https://github.com/gotohuman/n8n-nodes-gotohuman)

## Description

n8n node to request human reviews in AI workflows with gotoHuman

## Installation

```
@gotohuman/n8n-nodes-gotohuman
```

## Nodes (1)

### gotoHuman

- Node Type: `@gotohuman/n8n-nodes-gotohuman.gotoHuman`
- Version: 1
- Requires Credentials: Yes

Request human reviews with gotoHuman

#### Available Operations

- **Send and Wait for Response** (`sendAndWait`)
  Request a human review and wait for the response

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `resource` | options | Yes | `"reviewRequest"` |
| `metaSelect` | options | Yes | `"no"` |
| `assignToSelect` | options | Yes | `"all"` |
| `fields` | resourceMapper | Yes | `{"mappingMode":"defineBelow","value":null}` |
| `operation` | options | No | `"sendAndWait"` |
| `assignTo` | fixedCollection | No | `[]` |
| `metaKeyValues` | fixedCollection | No | `{}` |
| `additionalFields` | collection | No | `{}` |
| `reviewTemplateID` | resourceLocator | No | `{"mode":"list","value":""}` |
| `metaJson` | json | No | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "gotoHuman",
  "type": "@gotohuman/n8n-nodes-gotohuman.gotoHuman",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "resource": "reviewRequest",
    "metaSelect": "no",
    "assignToSelect": "all",
    "fields": {
      "mappingMode": "defineBelow",
      "value": null
    },
    "operation": "sendAndWait"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
