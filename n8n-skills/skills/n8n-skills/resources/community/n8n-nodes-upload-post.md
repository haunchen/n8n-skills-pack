# n8n-nodes-upload-post

## Basic Information

- Package: `n8n-nodes-upload-post`
- Category: 🔧 Utilities & Tools
- Version: 0.1.48
- Maintainer: upload-post
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-upload-post)
- Repository: [View Source](https://github.com/Upload-Post/n8n-nodes-upload-post)

## Description

n8n community node for Upload Post

## Installation

```
n8n-nodes-upload-post
```

## Nodes (1)

### Upload Post

- Node Type: `n8n-nodes-upload-post.uploadPost`
- Version: 1
- Requires Credentials: Yes

Upload content to social media via Upload-Post API

#### Available Operations

- **Upload Document** (`uploadDocument`)
  Upload a document (PDF, PPT, PPTX, DOC, DOCX) as a native carousel/viewer (Supports: LinkedIn only)
- **Upload Photo(s)** (`uploadPhotos`)
  Upload one or more photos (Supports: TikTok, Instagram, LinkedIn, Facebook, X, Threads)
- **Upload Text** (`uploadText`)
  Upload a text-based post (Supports: X, LinkedIn, Facebook, Threads)
- **Upload Video** (`uploadVideo`)
  Upload a single video (Supports: TikTok, Instagram, LinkedIn, YouTube, Facebook, X, Threads)

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `instagramUser` | options | Yes | `""` |
| `instagramPostId` | string | Yes | `""` |
| `instagramCommentId` | string | Yes | `""` |
| `instagramReplyMessage` | string | Yes | `""` |
| `user` | options | Yes | `""` |
| `userManual` | string | Yes | `""` |
| `platform` | multiOptions | Yes | `[]` |
| `photos` | string | Yes | `""` |
| `video` | string | Yes | `""` |
| `document` | string | Yes | `""` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Upload Post",
  "type": "n8n-nodes-upload-post.uploadPost",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "instagramUser": "",
    "instagramPostId": "",
    "instagramCommentId": "",
    "instagramReplyMessage": "",
    "user": "",
    "operation": "uploadDocument"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
