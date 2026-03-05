# n8n-nodes-a2a

## Basic Information

- Package: `n8n-nodes-a2a`
- Category: 📄 Document Processing
- Version: 0.4.0
- Maintainer: bruno.growthsales
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-a2a)
- Repository: [View Source](https://github.com/bruno-growthsales/n8n-nodes-a2a)

## Description

n8n community node for A2A (Account to Account) transfers, account management, and Google Agent2Agent protocol communication with advanced features including file upload, custom JSON fields, custom requests, and streaming support

## Installation

```
n8n-nodes-a2a
```

## Nodes (3)

### A2A

- Node Type: `n8n-nodes-a2a.a2a`
- Version: 1
- Requires Credentials: Yes

A2A (Account to Account) transfers, account management, and Agent2Agent protocol communication

#### Available Operations

- **Create** (`create`)
  Create a new transfer
- **Get** (`get`)
  Get a transfer by ID
- **Get Many** (`getMany`)
  Get multiple transfers
- **Cancel** (`cancel`)
  Cancel a transfer

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `currency` | options | Yes | `"USD"` |
| `transferId` | string | Yes | `""` |
| `amount` | number | Yes | `0` |
| `fromAccountId` | string | Yes | `""` |
| `toAccountId` | string | Yes | `""` |
| `accountId` | string | Yes | `""` |
| `agentUrl` | string | Yes | `""` |
| `message` | string | Yes | `""` |
| `customJsonMessage` | json | Yes | `"{\n  \"role\": \"user\",\n  \"parts\": [\n    {\n      \"type\": \"text\",\n      \"text\": \"Your message here\"\n    }\n  ]\n}"` |
| `customMethod` | string | Yes | `"tasks/send"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "A2A",
  "type": "n8n-nodes-a2a.a2a",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "currency": "USD",
    "transferId": "",
    "amount": 0,
    "fromAccountId": "",
    "toAccountId": "",
    "operation": "create"
  }
}
```

---

### Example Node

- Node Type: `n8n-nodes-a2a.exampleNode`
- Version: 1

Basic Example Node

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `myString` | string | No | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Example Node",
  "type": "n8n-nodes-a2a.exampleNode",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {}
}
```

---

### HttpBin

- Node Type: `n8n-nodes-a2a.httpBin`
- Version: 1
- Requires Credentials: Yes

Interact with HttpBin API

#### Available Operations

- **GET** (`get`)
  Perform a GET request
- **DELETE** (`delete`)
  Perform a DELETE request

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `typeofData` | options | Yes | `"queryParameter"` |
| `typeofData` | options | Yes | `"queryParameter"` |
| `resource` | options | No | `"httpVerb"` |
| `operation` | options | No | `"get"` |
| `arguments` | fixedCollection | No | `{}` |
| `arguments` | fixedCollection | No | `{}` |
| `arguments` | fixedCollection | No | `{}` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "HttpBin",
  "type": "n8n-nodes-a2a.httpBin",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "typeofData": "queryParameter",
    "operation": "get"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
