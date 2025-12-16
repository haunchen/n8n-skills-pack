# Data Transformation Nodes - Node Collection (Part 3)

This file contains complete information for 5 nodes.

## Table of Contents

- [Model Selector](#model-selector)
- [Tool Executor](#tool-executor)
- [Zep Vector Store](#zep-vector-store)
- [Zep Vector Store: Insert](#zep-vector-store-insert)
- [Zep Vector Store: Load](#zep-vector-store-load)

---

## Model Selector

## Basic Information

- Node Type: `nodes-langchain.modelSelector`
- Category: transform
- Package: @n8n/n8n-nodes-langchain

### Description

Use this node to select one of the connected models to this node based on workflow data

### Core Properties

| Property Name | Type | Required | Default | Description |
|---------|------|------|--------|------|
| `numberInputs` | options | No | `2` | The number of data inputs you want to merge. The node waits for all connected inputs to be executed. |
| `rules` | fixedCollection | No | `{}` | Rules to map workflow data to specific models |

#### Property Details

##### Number of Inputs (`numberInputs`)

The number of data inputs you want to merge. The node waits for all connected inputs to be executed.

Optional values:
- `2`: 2
- `3`: 3
- `4`: 4
- `5`: 5
- `6`: 6
- `7`: 7
- `8`: 8
- `9`: 9
- `10`: 10

##### Rules (`rules`)

Rules to map workflow data to specific models

Optional values:
- `undefined`: rule

### Connection Guide

### Connection Type

- Input Types: `main` (general data flow)
- Output Types: `ai_languageModel` (language Model)

### Can Receive From

1. Webhook - via `main` connection
2. ActiveCampaign Trigger - via `main` connection
3. Acuity Scheduling Trigger - via `main` connection
4. Affinity Trigger - via `main` connection
5. Airtable Trigger - via `main` connection
6. AMQP Trigger - via `main` connection
7. Asana Trigger - via `main` connection
8. Autopilot Trigger - via `main` connection
9. AWS SNS Trigger - via `main` connection
10. Bitbucket Trigger - via `main` connection

### Can Connect To

1. AI Agent - via `ai_languageModel` connection
2. Question and Answer Chain - via `ai_languageModel` connection
3. Sentiment Analysis - via `ai_languageModel` connection
4. Information Extractor - via `ai_languageModel` connection
5. Text Classifier - via `ai_languageModel` connection
6. Auto-fixing Output Parser - via `ai_languageModel` connection
7. Contextual Compression Retriever - via `ai_languageModel` connection
8. MultiQuery Retriever - via `ai_languageModel` connection
9. Vector Store Question Answer Tool - via `ai_languageModel` connection
### JSON Configuration Examples

#### Basic Configuration
```json
{
  "name": "Model Selector",
  "type": "nodes-langchain.modelSelector",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {}
}
```

---

## Tool Executor

## Basic Information

- Node Type: `nodes-langchain.toolExecutor`
- Category: transform
- Package: @n8n/n8n-nodes-langchain

### Description

Node to execute tools without an AI Agent

### Core Properties

| Property Name | Type | Required | Default | Description |
|---------|------|------|--------|------|
| `query` | json | No | `"{}"` | Parameters to pass to the tool as JSON or string |
| `toolName` | string | No | `""` | Name of the tool to execute if the connected tool is a toolkit |

### Connection Guide

### Connection Type

- Input Types: `main` (general data flow), `ai_tool` (tool)
- Output Types: `main` (general data flow)

### Can Receive From

1. Webhook - via `main` connection
2. ActiveCampaign Trigger - via `main` connection
3. Acuity Scheduling Trigger - via `main` connection
4. Affinity Trigger - via `main` connection
5. Airtable Trigger - via `main` connection
6. AMQP Trigger - via `main` connection
7. Asana Trigger - via `main` connection
8. Autopilot Trigger - via `main` connection
9. AWS SNS Trigger - via `main` connection
10. Bitbucket Trigger - via `main` connection

### Can Connect To

1. Code - via `main` connection
2. Function - via `main` connection
3. HTTP Request - via `main` connection
4. If - via `main` connection
5. Set - via `main` connection
6. Merge - via `main` connection
7. Airtable - via `main` connection
8. Discord - via `main` connection
9. Dropbox - via `main` connection
10. GitHub - via `main` connection

### Special Requirements

This AI node requires the following special inputs:

- tool (optional, multiple allowed)
### JSON Configuration Examples

#### Basic Configuration
```json
{
  "name": "Tool Executor",
  "type": "nodes-langchain.toolExecutor",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {}
}
```

---

## Zep Vector Store

## Basic Information

- Node Type: `nodes-langchain.vectorStoreZep`
- Category: transform
- Package: @n8n/n8n-nodes-langchain
- Requires Credentials: Yes

### Description

Work with your data in Zep Vector Store

### Core Properties

| Property Name | Type | Required | Default | Description |
|---------|------|------|--------|------|
| `toolName` | string | Yes | `""` | Name of the vector store |
| `toolDescription` | string | Yes | `""` | Explain to the LLM what this tool does, a good, specific description would allow LLMs to produce expected results much more often |
| `prompt` | string | Yes | `""` | Search prompt to retrieve matching documents from the vector store using similarity-based ranking |
| `id` | string | Yes | `""` | ID of an embedding entry |
| `collectionName` | string | Yes | `""` | - |
| `mode` | options | No | `"retrieve"` | - |
| `options` | collection | No | `{}` | - |
| `options` | collection | No | `{}` | - |
| `options` | collection | No | `{}` | - |
| `embeddingBatchSize` | number | No | `200` | Number of documents to embed in a single batch |

#### Property Details

##### Operation Mode (`mode`)

Optional values:
- `load`: Get Many - Get many ranked documents from vector store for query
- `insert`: Insert Documents - Insert documents into vector store
- `retrieve`: Retrieve Documents (As Vector Store for Chain/Tool) - Retrieve documents from vector store to be used as vector store with AI nodes
- `retrieve-as-tool`: Retrieve Documents (As Tool for AI Agent) - Retrieve documents from vector store to be used as tool with AI nodes

##### Options (`options`)

Optional values:
- `undefined`: embeddingDimensions - Whether to allow using characters from the Unicode surrogate blocks
- `undefined`: isAutoEmbedded - Whether to automatically embed documents when they are added

##### Options (`options`)

Optional values:
- `undefined`: embeddingDimensions - Whether to allow using characters from the Unicode surrogate blocks
- `undefined`: metadata - Metadata to filter the document by

##### Options (`options`)

Optional values:
- `undefined`: embeddingDimensions - Whether to allow using characters from the Unicode surrogate blocks
- `undefined`: metadata - Metadata to filter the document by

### Connection Guide

### Connection Type

- Input Types: `main` (general data flow)
- Output Types: `main` (general data flow)
- Output Count: 0 (configurable)

### Can Receive From

1. Webhook - via `main` connection
2. ActiveCampaign Trigger - via `main` connection
3. Acuity Scheduling Trigger - via `main` connection
4. Affinity Trigger - via `main` connection
5. Airtable Trigger - via `main` connection
6. AMQP Trigger - via `main` connection
7. Asana Trigger - via `main` connection
8. Autopilot Trigger - via `main` connection
9. AWS SNS Trigger - via `main` connection
10. Bitbucket Trigger - via `main` connection

### Can Connect To

1. Code - via `main` connection
2. Function - via `main` connection
3. HTTP Request - via `main` connection
4. If - via `main` connection
5. Set - via `main` connection
6. Merge - via `main` connection
7. Airtable - via `main` connection
8. Discord - via `main` connection
9. Dropbox - via `main` connection
10. GitHub - via `main` connection
### JSON Configuration Examples

#### Basic Configuration
```json
{
  "name": "Zep Vector Store",
  "type": "nodes-langchain.vectorStoreZep",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "toolName": "",
    "toolDescription": "",
    "prompt": "",
    "id": "",
    "collectionName": ""
  }
}
```

---

## Zep Vector Store: Insert

## Basic Information

- Node Type: `nodes-langchain.vectorStoreZepInsert`
- Category: transform
- Package: @n8n/n8n-nodes-langchain
- Requires Credentials: Yes

### Description

Insert data into Zep Vector Store index

### Core Properties

| Property Name | Type | Required | Default | Description |
|---------|------|------|--------|------|
| `collectionName` | string | Yes | `""` | - |
| `options` | collection | No | `{}` | - |
| `deprecationNotice` | notice | No | `""` | - |
| `notice` | notice | No | `""` | - |

#### Property Details

##### Options (`options`)

Optional values:
- `undefined`: embeddingDimensions - Whether to allow using characters from the Unicode surrogate blocks
- `undefined`: isAutoEmbedded - Whether to automatically embed documents when they are added

### Connection Guide

### Connection Type

- Input Types: `main` (general data flow), `ai_document` (document), `ai_embedding` (embedding)
- Output Types: `main` (general data flow)

### Can Receive From

1. Webhook - via `main` connection
2. ActiveCampaign Trigger - via `main` connection
3. Acuity Scheduling Trigger - via `main` connection
4. Affinity Trigger - via `main` connection
5. Airtable Trigger - via `main` connection
6. AMQP Trigger - via `main` connection
7. Asana Trigger - via `main` connection
8. Autopilot Trigger - via `main` connection
9. AWS SNS Trigger - via `main` connection
10. Bitbucket Trigger - via `main` connection

### Can Connect To

1. Code - via `main` connection
2. Function - via `main` connection
3. HTTP Request - via `main` connection
4. If - via `main` connection
5. Set - via `main` connection
6. Merge - via `main` connection
7. Airtable - via `main` connection
8. Discord - via `main` connection
9. Dropbox - via `main` connection
10. GitHub - via `main` connection

### Special Requirements

This AI node requires the following special inputs:

- document (optional)
- embedding (optional)
### JSON Configuration Examples

#### Basic Configuration
```json
{
  "name": "Zep Vector Store: Insert",
  "type": "nodes-langchain.vectorStoreZepInsert",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "collectionName": ""
  }
}
```

---

## Zep Vector Store: Load

## Basic Information

- Node Type: `nodes-langchain.vectorStoreZepLoad`
- Category: transform
- Package: @n8n/n8n-nodes-langchain
- Requires Credentials: Yes

### Description

Load data from Zep Vector Store index

### Core Properties

| Property Name | Type | Required | Default | Description |
|---------|------|------|--------|------|
| `collectionName` | string | Yes | `""` | - |
| `options` | collection | No | `{}` | - |
| `deprecationNotice` | notice | No | `""` | - |

#### Property Details

##### Options (`options`)

Optional values:
- `undefined`: embeddingDimensions - Whether to allow using characters from the Unicode surrogate blocks
- `undefined`: metadata - Metadata to filter the document by

### Connection Guide

### Connection Type

- Input Types: `ai_embedding` (embedding)
- Output Types: `ai_vectorStore` (vector Store)

### Can Receive From

1. Embeddings Cohere - via `ai_embedding` connection
2. Embeddings AWS Bedrock - via `ai_embedding` connection
3. Embeddings Azure OpenAI - via `ai_embedding` connection
4. Embeddings Google Gemini - via `ai_embedding` connection
5. Embeddings Google Vertex - via `ai_embedding` connection
6. Embeddings Hugging Face Inference - via `ai_embedding` connection
7. Embeddings Mistral Cloud - via `ai_embedding` connection
8. Embeddings OpenAI - via `ai_embedding` connection
9. Embeddings Lemonade - via `ai_embedding` connection
10. Embeddings Ollama - via `ai_embedding` connection

### Can Connect To

1. Vector Store Retriever - via `ai_vectorStore` connection
2. Vector Store Question Answer Tool - via `ai_vectorStore` connection

### Special Requirements

This AI node requires the following special inputs:

- embedding (optional)
### JSON Configuration Examples

#### Basic Configuration
```json
{
  "name": "Zep Vector Store: Load",
  "type": "nodes-langchain.vectorStoreZepLoad",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "collectionName": ""
  }
}
```
