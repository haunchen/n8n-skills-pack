# n8n-nodes-pdf4me

## Basic Information

- Package: `n8n-nodes-pdf4me`
- Category: 📄 Document Processing
- Version: 2.3.1
- Maintainer: GitHub Actions
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-pdf4me)
- Repository: [View Source](https://github.com/pdf4me/n8n-nodes-pdf4me)

## Description

n8n community node for PDF4me API integration

## Installation

```
n8n-nodes-pdf4me
```

## Nodes (1)

### PDF4me

- Node Type: `n8n-nodes-pdf4me.PDF4me`
- Version: 1
- Requires Credentials: Yes

Comprehensive PDF and document processing: generate barcodes, convert files, extract data, manipulate images, and automate workflows with the PDF4ME API

#### Available Operations

- **AI-Invoice Parser** (`AI-Invoice Parser`)
  Extract structured data from invoices using AI/ML technology for automated data entry
- **AI-Process Bank Cheque** (`AI-Process Bank Cheque`)
  Extract structured data from bank cheques using AI/ML technology for payment processing
- **AI-Process Credit Card** (`AI-Process Credit Card`)
  Extract structured data from credit cards using AI/ML technology for payment processing
- **AI-Process Contract** (`AI-Process Contract`)
  Extract structured data from contracts using AI/ML technology for legal document analysis
- **AI-Process HealthCard** (`AI-Process HealthCard`)
  Extract structured data from health cards using AI/ML technology for member management
- **AI-Process Marriage Certificate** (`AI-Process Marriage Certificate`)
  Extract structured data from marriage certificates using AI/ML technology for document verification
- **AI-Process Mortgage Document** (`AI-Process Mortgage Document`)
  Extract structured data from mortgage documents using AI/ML technology for loan processing
- **AI-Process Pay Stub** (`AI-Process Pay Stub`)
  Extract structured data from pay stubs using AI/ML technology for payroll processing
- **AI Auto Crop Document** (`AI Auto Crop Document`)
  Automatically crop a document using AI to remove borders and unwanted areas
- **AI - Universal Document Data Extraction** (`Process Universal Document`)
  Extract specified fields from documents using universal document processing
- ... and 5 more operations

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `inputDataType` | options | Yes | `"binaryData"` |
| `inputDataType` | options | Yes | `"binaryData"` |
| `barcodeType` | options | Yes | `"qrCode"` |
| `alignX` | options | Yes | `"Right"` |
| `alignY` | options | Yes | `"Bottom"` |
| `pdfInputDataType` | options | Yes | `"binaryData"` |
| `formFieldType` | options | Yes | `"TextBox"` |
| `inputDataType` | options | Yes | `"binaryData"` |
| `location` | options | Yes | `"Header"` |
| `inputDataType` | options | Yes | `"binaryData"` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "PDF4me",
  "type": "n8n-nodes-pdf4me.PDF4me",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "inputDataType": "binaryData",
    "barcodeType": "qrCode",
    "alignX": "Right",
    "alignY": "Bottom",
    "operation": "AI-Invoice Parser"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
