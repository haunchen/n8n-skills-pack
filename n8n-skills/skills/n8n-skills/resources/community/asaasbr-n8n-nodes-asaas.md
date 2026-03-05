# @asaasbr/n8n-nodes-asaas

## Basic Information

- Package: `@asaasbr/n8n-nodes-asaas`
- Category: 🔧 Utilities & Tools
- Version: 1.0.3
- Maintainer: phelipe_pereira
- npm: [View Package](https://www.npmjs.com/package/@asaasbr/n8n-nodes-asaas)
- Repository: [View Source](https://github.com/asaasdev/n8n-plugin-asaas)

## Description

n8n nodes for integrating with the Asaas API

## Installation

```
@asaasbr/n8n-nodes-asaas
```

## Nodes (1)

### Asaas

- Node Type: `@asaasbr/n8n-nodes-asaas.asaas`
- Version: 1
- Requires Credentials: Yes

Interagir com a API do Asaas

#### Available Operations

- **Atualizar Cliente Existente** (`update`)
  Atualizar um cliente
- **Criar Novo Cliente** (`create`)
  Criar um novo cliente
- **Get Many** (`getAll`)
  Listar todos os clientes
- **Recuperar Notificações De Um Cliente** (`getNotifications`)
- **Recuperar Um Único Cliente** (`get`)
  Buscar um cliente específico
- **Remover Cliente** (`delete`)
  Excluir um cliente
- **Restaurar Cliente Removido** (`restore`)
  Restaurar um cliente excluído

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `value` | number | Yes | `0` |
| `value` | number | Yes | `0` |
| `value` | number | Yes | `0` |
| `value` | number | Yes | `0` |
| `url` | string | Yes | `""` |
| `value` | number | Yes | `0` |
| `sendType` | options | Yes | `"NON_SEQUENTIALLY"` |
| `events` | multiOptions | Yes | `[]` |
| `keyType` | options | Yes | `"EVP"` |
| `billingType` | options | Yes | `"BOLETO"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Asaas",
  "type": "@asaasbr/n8n-nodes-asaas.asaas",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "value": 0,
    "url": "",
    "operation": "update"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
