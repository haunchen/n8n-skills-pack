# n8n-nodes-efibank

## Basic Information

- Package: `n8n-nodes-efibank`
- Category: 🔧 Utilities & Tools
- Version: 1.0.10
- Maintainer: consultoria-efi
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-efibank)
- Repository: [View Source](https://github.com/efipay/n8n-nodes-efibank)

## Description

Nó personalizado para integração com as APIs Cobranças e Pix do Efi Bank, permitindo operações de pagamentos, recebimentos e gerenciamento de transações financeiras.

## Installation

```
n8n-nodes-efibank
```

## Nodes (2)

### Efí Bank | API Cobranças

- Node Type: `n8n-nodes-efibank.EfiBankCobrancas`
- Version: 1
- Requires Credentials: Yes

Integração com a API Cobranças do Efí Bank

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `brand` | options | Yes | `"mastercard"` |
| `charge_id` | string | Yes | `""` |
| `begin_date` | string | Yes | `"2025-01-01"` |
| `end_date` | string | Yes | `"2025-12-31"` |
| `requestBodyAlterarVencimento` | string | Yes | `""` |
| `email` | string | Yes | `""` |
| `requestBodyHistorico` | string | Yes | `""` |
| `charge_id` | string | Yes | `""` |
| `amount` | number | Yes | `null` |
| `begin_date` | string | Yes | `"2025-01-01"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Efí Bank | API Cobranças",
  "type": "n8n-nodes-efibank.EfiBankCobrancas",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "brand": "mastercard",
    "charge_id": "",
    "begin_date": "2025-01-01",
    "end_date": "2025-12-31",
    "requestBodyAlterarVencimento": ""
  }
}
```

---

### Efí Bank | API Pix

- Node Type: `n8n-nodes-efibank.EfiBankPix`
- Version: 1
- Requires Credentials: Yes

Integração com a API Pix da Efí Bank

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `txid` | string | Yes | `""` |
| `inicio` | string | Yes | `"2025-01-01T00:00:00Z"` |
| `fim` | string | Yes | `"2025-12-31T23:59:59Z"` |
| `inicio` | string | Yes | `"2025-01-01T00:00:00Z"` |
| `fim` | string | Yes | `"2025-12-31T23:59:59Z"` |
| `inicio` | string | Yes | `"2025-01-01T00:00:00Z"` |
| `fim` | string | Yes | `"2025-12-31T23:59:59Z"` |
| `pixCopiaECola` | string | Yes | `""` |
| `inicio` | string | Yes | `"2025-01-01T00:00:00Z"` |
| `fim` | string | Yes | `"2025-12-31T23:59:59Z"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Efí Bank | API Pix",
  "type": "n8n-nodes-efibank.EfiBankPix",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "txid": "",
    "inicio": "2025-01-01T00:00:00Z",
    "fim": "2025-12-31T23:59:59Z"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
