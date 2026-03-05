# n8n-nodes-pdfco

## Basic Information

- Package: `n8n-nodes-pdfco`
- Category: 📄 Document Processing
- Version: 1.0.6
- Maintainer: artifex-dev
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-pdfco)
- Repository: [View Source](https://github.com/pdfdotco/n8n-nodes-pdfco)

## Description

Pdf.co nodes for n8n

## Installation

```
n8n-nodes-pdfco
```

## Nodes (1)

### PDF.co Api

- Node Type: `n8n-nodes-pdfco.PDFco Api`
- Version: 1
- Requires Credentials: Yes

Generate PDF, extract data from PDF, split PDF, merge PDF, convert PDF. Fill PDF forms, add text and images to pdf and much more with pdf.co!

#### Available Operations

- **AI Invoice Parser** (`AI Invoice Parser`)
  Transform your invoice processing with our advanced AI. Enjoy quick, accurate data extraction that eliminates manual effort and saves you valuable time.
- **URL/HTML to PDF** (`URL/HTML to PDF`)
  Convert HTML or URL to PDF with advanced options (e.g. layout, orientation). Supports HTML templates (Handlebar and Mustache).
- **Merge PDF** (`Merge PDF`)
  Combine multiple document formats into a single PDF. Supported formats include PDF, DOC, DOCX, XLS, JPG, PNG, and more.
- **Split PDF** (`Split PDF`)
  PDF Splitter that takes PDF file and splits into multiple PDF files using page index, page range, text search or barcode search
- **Convert To PDF** (`Convert to PDF`)
  Convert a variety of formats such as URLs, HTML code, documents, spreadsheets, presentations, images, and more into PDF
- **Convert From PDF** (`Convert from PDF`)
  Convert PDF pages to structured CSV, XML, JSON, Plain Text, Convert PDF to JPG, PDF to PNG, PDF to TIFF, and more
- **Add Text/Images to PDF** (`Add Text/Images to PDF`)
  Add text, images, and annotations to PDF documents with precise positioning and styling options
- **Fill a PDF Form** (`Fill a PDF Form`)
  Fill interactive PDF forms with text, checkboxes, and other form elements
- **PDF Information & Form Fields** (`PDF Information & Form Fields`)
  Extract metadata and form field information from PDF documents
- **Compress PDF** (`Compress PDF`)
  Reduce PDF file size while maintaining quality
- ... and 9 more operations

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `[]` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |
| `url` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "PDF.co Api",
  "type": "n8n-nodes-pdfco.PDFco Api",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "url": "",
    "operation": "AI Invoice Parser"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
