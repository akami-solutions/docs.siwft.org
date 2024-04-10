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

## Caching

Since the `04152024-001` release, the output is cached on the server side for some endpoints. The cache is currently 300 seconds. To prevent the server-side cache use the `Pragma: no-cache` header in your GET request

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

## How to get digital assets

> WARNING!<br/>
> This area is under construction
{style="warning"}

### As a Wallet Hub

Upon receiving a Wallet Hub from SIWFT, the said Wallet Hub will be continuously provided with Digital Assets by SIWFT.

This credit will only be offered by SIWFT until they deem that there are enough Digital Assets in circulation. Once this is achieved, the respective Wallethubs will be informed accordingly.

### Restrictions

Wallet Hubs are not allowed to spend this credit for anything other than their customers. This can include:

* Welcome Bonus
* Giveaway (only after 100-200 Wallets)
* Others upon request

It should also be noted that the credit should not only go to a few people, but to several.
### As a Wallet Holder

SIWFT is not authorized to credit individual wallets or make changes to a wallet without a legitimate reason. However, Wallet Hubs are authorized to restrict your wallet and its rights.
> Info<br/>
> If you notice that your wallet hub violates our guidelines, violates rights or is otherwise bad or strange, you can inform SIWFT at any time via [e-mail](mailto:abuse@siwft.org).
{style="info"}