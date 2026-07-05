# n8n-nodes-yepcode

## Basic Information

- Package: `n8n-nodes-yepcode`
- Category: 🔧 Utilities & Tools
- Version: 1.1.0
- Maintainer: yepcode
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-yepcode)
- Repository: [View Source](https://github.com/yepcode/n8n-nodes-yepcode)

## Description

Custom n8n node module for YepCode

## Installation

```
n8n-nodes-yepcode
```

## Nodes (1)

### YepCode

- Node Type: `n8n-nodes-yepcode.yepCode`
- Version: 1
- Requires Credentials: Yes

YepCode lets you run full processes or dynamic scripts using Node.js or Python, with support for any NPM or PyPI dependency. All in a secure, sandboxed environment.

#### Available Operations

- **Run Process** (`run_process`)
  Move your complex business logic into yep code processes and trigger them from your workflows using dynamic input parameters it s the most flexible way to connect with your ap is and services using real code with zero dev ops overhead
- **Run Code** (`run_code`)
  A lightweight, flexible way to execute Node.js or Python code on demand — directly from your workflows or AI agents. The run_code tool runs in secure cloud sandboxes with full support for NPM and PyPI dependencies (https://yepcode.io/docs/dependencies), access to secrets, APIs, and databases. Perfect for quick scripts, dynamic logic, or AI-generated code.

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `process` | options | Yes | `""` |
| `code` | string | Yes | `"// Import any npm package - YepCode will install it automatically\nconst { DateTime } = require(\"luxon\");\n\nconst { n8n } = yepcode.context.parameters;\n\nconst results = [];\nfor (const item of n8n.items) {\n  results.push({\n    ...item.json,\n    processedAt: DateTime.now().toISO(),\n  });\n}\n\n// Access n8n metadata - check all available fields at: https://docs.n8n.io/code/builtin/n8n-metadata/\nconsole.log(\"Environment:\", n8n.metadata);\nconsole.log(\"Resume URL:\", n8n.metadata[\"$execution\"].resumeUrl);\n\nreturn results;"` |
| `operation` | options | No | `"run_process"` |
| `language` | options | No | `""` |
| `mode` | options | No | `"runOnceForAllItems"` |
| `mode` | options | No | `"runOnceForAllItems"` |
| `parameters` | resourceMapper | No | `{"mappingMode":"defineBelow","value":null}` |
| `addN8nContext` | boolean | No | `true` |
| `version` | options | No | `"$CURRENT"` |
| `synchronous` | boolean | No | `true` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "YepCode",
  "type": "n8n-nodes-yepcode.yepCode",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "process": "",
    "code": "// Import any npm package - YepCode will install it automatically\nconst { DateTime } = require(\"luxon\");\n\nconst { n8n } = yepcode.context.parameters;\n\nconst results = [];\nfor (const item of n8n.items) {\n  results.push({\n    ...item.json,\n    processedAt: DateTime.now().toISO(),\n  });\n}\n\n// Access n8n metadata - check all available fields at: https://docs.n8n.io/code/builtin/n8n-metadata/\nconsole.log(\"Environment:\", n8n.metadata);\nconsole.log(\"Resume URL:\", n8n.metadata[\"$execution\"].resumeUrl);\n\nreturn results;",
    "operation": "run_process"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
