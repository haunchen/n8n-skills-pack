# n8n-nodes-weld

## Basic Information

- Package: `n8n-nodes-weld`
- Category: 🔧 Utilities & Tools
- Version: 1.1.4
- Maintainer: GitHub Actions
- npm: [View Package](https://www.npmjs.com/package/n8n-nodes-weld)
- Repository: [View Source](https://github.com/useweld/n8n-nodes-weld)

## Description

n8n community node for Weld — web scraping across LinkedIn, Instagram, TikTok, Twitter/X, YouTube & Facebook

## Installation

```
n8n-nodes-weld
```

## Nodes (24)

### Weld Jobs

- Node Type: `n8n-nodes-weld.weldJobs`
- Version: 1
- Requires Credentials: Yes

Manage Weld scrape jobs and credits — list, cancel, check status, and view balance

#### Available Operations

- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job
- **List** (`list`)
  List recent scrape jobs
- **Cancel** (`cancel`)
  Cancel a pending or processing job and refund credits

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `jobId` | string | Yes | `""` |
| `resource` | options | No | `"job"` |
| `operation` | options | No | `"list"` |
| `operation` | options | No | `"getBalance"` |
| `statusFilter` | options | No | `""` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |
| `transactionLimit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Jobs",
  "type": "n8n-nodes-weld.weldJobs",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "jobId": "",
    "operation": "get"
  }
}
```

---

### Weld LinkedIn Profiles

- Node Type: `n8n-nodes-weld.weldLinkedInProfiles`
- Version: 1
- Requires Credentials: Yes

Extract professional profile data from LinkedIn profile URLs

#### Available Operations

- **Create** (`create`)
  Extract professional profile data from LinkedIn profile URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld LinkedIn Profiles",
  "type": "n8n-nodes-weld.weldLinkedInProfiles",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld LinkedIn Companies

- Node Type: `n8n-nodes-weld.weldLinkedInCompanies`
- Version: 1
- Requires Credentials: Yes

Extract company data from LinkedIn company page URLs

#### Available Operations

- **Create** (`create`)
  Extract company data from LinkedIn company page URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld LinkedIn Companies",
  "type": "n8n-nodes-weld.weldLinkedInCompanies",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld LinkedIn Posts

- Node Type: `n8n-nodes-weld.weldLinkedInPosts`
- Version: 1
- Requires Credentials: Yes

Extract posts with engagement metrics from LinkedIn profile, company, or post URLs

#### Available Operations

- **Create** (`create`)
  Extract posts with engagement metrics from LinkedIn profile, company, or post URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld LinkedIn Posts",
  "type": "n8n-nodes-weld.weldLinkedInPosts",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Instagram Profiles

- Node Type: `n8n-nodes-weld.weldInstagramProfiles`
- Version: 1
- Requires Credentials: Yes

Extract profile data from Instagram user URLs

#### Available Operations

- **Create** (`create`)
  Extract profile data from Instagram user URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Instagram Profiles",
  "type": "n8n-nodes-weld.weldInstagramProfiles",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Instagram Posts

- Node Type: `n8n-nodes-weld.weldInstagramPosts`
- Version: 1
- Requires Credentials: Yes

Extract posts with media data from Instagram post URLs

#### Available Operations

- **Create** (`create`)
  Extract posts with media data from Instagram post URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Instagram Posts",
  "type": "n8n-nodes-weld.weldInstagramPosts",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Instagram Comments

- Node Type: `n8n-nodes-weld.weldInstagramComments`
- Version: 1
- Requires Credentials: Yes

Extract comments from Instagram post URLs

#### Available Operations

- **Create** (`create`)
  Extract comments from Instagram post URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Instagram Comments",
  "type": "n8n-nodes-weld.weldInstagramComments",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld TikTok Profiles

- Node Type: `n8n-nodes-weld.weldTikTokProfiles`
- Version: 1
- Requires Credentials: Yes

Extract creator profile data from TikTok user URLs

#### Available Operations

- **Create** (`create`)
  Extract creator profile data from TikTok user URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld TikTok Profiles",
  "type": "n8n-nodes-weld.weldTikTokProfiles",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld TikTok Videos

- Node Type: `n8n-nodes-weld.weldTikTokVideos`
- Version: 1
- Requires Credentials: Yes

Extract video data from TikTok video URLs

#### Available Operations

- **Create** (`create`)
  Extract video data from TikTok video URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld TikTok Videos",
  "type": "n8n-nodes-weld.weldTikTokVideos",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Twitter/X Profiles

- Node Type: `n8n-nodes-weld.weldTwitterProfiles`
- Version: 1
- Requires Credentials: Yes

Extract profile data from Twitter/X user URLs

#### Available Operations

- **Create** (`create`)
  Extract profile data from Twitter/X user URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Twitter/X Profiles",
  "type": "n8n-nodes-weld.weldTwitterProfiles",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Twitter/X Posts

- Node Type: `n8n-nodes-weld.weldTwitterPosts`
- Version: 1
- Requires Credentials: Yes

Extract tweets from Twitter/X post URLs

#### Available Operations

- **Create** (`create`)
  Extract tweets from Twitter/X post URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Twitter/X Posts",
  "type": "n8n-nodes-weld.weldTwitterPosts",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld YouTube Channels

- Node Type: `n8n-nodes-weld.weldYouTubeChannels`
- Version: 1
- Requires Credentials: Yes

Extract channel data from YouTube channel URLs

#### Available Operations

- **Create** (`create`)
  Extract channel data from YouTube channel URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld YouTube Channels",
  "type": "n8n-nodes-weld.weldYouTubeChannels",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld YouTube Comments

- Node Type: `n8n-nodes-weld.weldYouTubeComments`
- Version: 1
- Requires Credentials: Yes

Extract comments from YouTube video URLs

#### Available Operations

- **Create** (`create`)
  Extract comments from YouTube video URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld YouTube Comments",
  "type": "n8n-nodes-weld.weldYouTubeComments",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Facebook Profiles

- Node Type: `n8n-nodes-weld.weldFacebookProfiles`
- Version: 1
- Requires Credentials: Yes

Extract profile and post data from Facebook profile URLs

#### Available Operations

- **Create** (`create`)
  Extract profile and post data from Facebook profile URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Facebook Profiles",
  "type": "n8n-nodes-weld.weldFacebookProfiles",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Facebook Groups

- Node Type: `n8n-nodes-weld.weldFacebookGroups`
- Version: 1
- Requires Credentials: Yes

Extract group posts from Facebook group URLs

#### Available Operations

- **Create** (`create`)
  Extract group posts from Facebook group URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Facebook Groups",
  "type": "n8n-nodes-weld.weldFacebookGroups",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Indeed Jobs

- Node Type: `n8n-nodes-weld.weldIndeedJobs`
- Version: 1
- Requires Credentials: Yes

Extract job postings from Indeed job listing URLs

#### Available Operations

- **Create** (`create`)
  Extract job postings from Indeed job listing URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Indeed Jobs",
  "type": "n8n-nodes-weld.weldIndeedJobs",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Indeed Companies

- Node Type: `n8n-nodes-weld.weldIndeedCompanies`
- Version: 1
- Requires Credentials: Yes

Extract company reviews and ratings from Indeed company pages

#### Available Operations

- **Create** (`create`)
  Extract company reviews and ratings from Indeed company pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Indeed Companies",
  "type": "n8n-nodes-weld.weldIndeedCompanies",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Glassdoor Companies

- Node Type: `n8n-nodes-weld.weldGlassdoorCompanies`
- Version: 1
- Requires Credentials: Yes

Extract company profiles with ratings from Glassdoor company pages

#### Available Operations

- **Create** (`create`)
  Extract company profiles with ratings from Glassdoor company pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Glassdoor Companies",
  "type": "n8n-nodes-weld.weldGlassdoorCompanies",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Glassdoor Reviews

- Node Type: `n8n-nodes-weld.weldGlassdoorReviews`
- Version: 1
- Requires Credentials: Yes

Extract employee reviews from Glassdoor review pages

#### Available Operations

- **Create** (`create`)
  Extract employee reviews from Glassdoor review pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Glassdoor Reviews",
  "type": "n8n-nodes-weld.weldGlassdoorReviews",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Glassdoor Jobs

- Node Type: `n8n-nodes-weld.weldGlassdoorJobs`
- Version: 1
- Requires Credentials: Yes

Extract job listings with salary estimates from Glassdoor job pages

#### Available Operations

- **Create** (`create`)
  Extract job listings with salary estimates from Glassdoor job pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Glassdoor Jobs",
  "type": "n8n-nodes-weld.weldGlassdoorJobs",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Yelp Businesses

- Node Type: `n8n-nodes-weld.weldYelpBusinesses`
- Version: 1
- Requires Credentials: Yes

Extract business profiles with ratings from Yelp business pages

#### Available Operations

- **Create** (`create`)
  Extract business profiles with ratings from Yelp business pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Yelp Businesses",
  "type": "n8n-nodes-weld.weldYelpBusinesses",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Yelp Reviews

- Node Type: `n8n-nodes-weld.weldYelpReviews`
- Version: 1
- Requires Credentials: Yes

Extract customer reviews from Yelp business review pages

#### Available Operations

- **Create** (`create`)
  Extract customer reviews from Yelp business review pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Yelp Reviews",
  "type": "n8n-nodes-weld.weldYelpReviews",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld GitHub Repositories

- Node Type: `n8n-nodes-weld.weldGitHubRepositories`
- Version: 1
- Requires Credentials: Yes

Extract repository data from GitHub repository URLs

#### Available Operations

- **Create** (`create`)
  Extract repository data from GitHub repository URLs
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld GitHub Repositories",
  "type": "n8n-nodes-weld.weldGitHubRepositories",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

### Weld Crunchbase Companies

- Node Type: `n8n-nodes-weld.weldCrunchbaseCompanies`
- Version: 1
- Requires Credentials: Yes

Extract company data with funding information from Crunchbase company pages

#### Available Operations

- **Create** (`create`)
  Extract company data with funding information from Crunchbase company pages
- **Get** (`get`)
  Get job status and details by ID
- **Get Results** (`getResults`)
  Get results from a completed job

#### Core Properties

| Property | Type | Required | Default |
|----------|------|----------|---------|
| `urls` | string | Yes | `""` |
| `jobId` | string | Yes | `""` |
| `operation` | options | No | `"create"` |
| `jobName` | string | No | `""` |
| `waitForCompletion` | boolean | No | `false` |
| `pollInterval` | number | No | `10` |
| `maxWait` | number | No | `300` |
| `resultLimit` | number | No | `1000` |
| `returnAll` | boolean | No | `false` |
| `limit` | number | No | `50` |

#### Connection

- Input Types: `main`
- Output Types: `main`

#### Example Configuration

```json
{
  "name": "Weld Crunchbase Companies",
  "type": "n8n-nodes-weld.weldCrunchbaseCompanies",
  "typeVersion": 1,
  "position": [
    250,
    300
  ],
  "parameters": {
    "urls": "",
    "jobId": "",
    "operation": "create"
  }
}
```

---

---

[← Back to Community Nodes Index](README.md)
