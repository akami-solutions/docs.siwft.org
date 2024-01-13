# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

The SIWFT API documentation should help you to better understand our API so that you can use our API as well as possible
## What you can do using SIWFT

With the SIWFT API you can create transactions within the SIWFT Economy and also manage them to whom and from whom
## Authentication

The SIWFT is an open API, which means that we make the most important data you need available to everyone as long as it is not private data. For this you need an API key and sometimes also the username of the wallet
## Base URL

The API requests are carried out with the URL https://api.siwft.org

## Rate Limiting

As of 13.01.2024 the rate limit settings are 100 requests per 10 seconds

## Error Handling

The SIWFT has a specific error handling scheme which looks as follows:

### Fehlerhafte Anfrage:

```json
{
  "success": false,
  "error": {
    "0": {
      "message": "Error Message",
      "code": 500
    }
  }
}
```

## Versioning

Our versioning always starts with a "v" followed by a number.
Each new version contains an API change that includes new features or no longer has them.

<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>
