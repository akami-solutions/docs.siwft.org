# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
If you already have a wallet, you can also use your wallet data to test the API for yourself

## Prerequisites

To create your first request, you need the following data that you should have received from your Wallet Hub

* Your IWAN
* Your wallet key
* Your username

## Authentication

There are two ways in which you can process the request.
To request only public data, you don't need your username or wallet key, just your IWAN.
However, if you want to have all data then both data are required

## Making Your First Request

```http
GET /v0/wallet/:IWAN HTTP/1.1
Host: api.siwft.org
Authorization: YOUR_ACCESS_TOKEN
X-Auth-Username: YOUR_USERNAME
```

## Response Handling

If the request is successful, you should see a response with similar data:

```json
{
  "success": true,
  "message": {
    "username": "Your Username",
    "isActive": true,
    "isEnterprise": false,
    "balance": "0.48",
    "key": "key_h246375h24672510ffj8g3hh24678g2467dz4275"
  }
}
```

If you have not defined a username or authorization, the key would be set to "null"