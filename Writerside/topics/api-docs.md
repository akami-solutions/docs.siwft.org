# API Overview

<!-- This document provides an introduction into your API. -->
## What is SIWFT?

SIWFT is an API endpoint that enables the creation and processing of online transactions without any connection to real-world currencies like euros, dollars, etc. Using this API, you can create wallet hubs, wallets, and process and verify transactions. SIWFT serves as the central endpoint for handling digital transactions that do not involve physical goods, content, or real money.

## Do we work with SWIFT?

**__No, we do not.__** We are not affiliated with SWIFT and do not utilize their endpoints or services.

## Why SIWFT and how did it come about?

The concept of SIWFT emerged in connection with the popular online chat platform Discord Inc. The idea was to develop a centralized system that resembles the real-world financial system, providing younger generations with a practical understanding of how it operates.

## Deeper Understanding and Comparison to the Real World

Due to legal restrictions, we have guidelines for naming specific entities. For reference, please refer to the table below:

| SIWFT Term     | Real-World Term    |
|----------------|--------------------|
| Wallet Hub     | Bank               |
| Wallet         | Account            |
| Digital Asset  | Currency           |

We hope this improved version of the text provides a clearer understanding of SIWFT and its purpose.


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
