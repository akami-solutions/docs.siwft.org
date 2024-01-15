# Transactions
<code-block lang="mermaid">
---
title: Transaction creation
---
sequenceDiagram
Wallet->>+Wallet Hub: Requests a transaction
Wallet Hub->>SIWFT: Sends the necessary data to SIWFT
SIWFT->>Wallet Hub: Processes the transaction and responds with useful data
Wallet Hub->>+Wallet: Passes on that the transaction was successful or not.
</code-block>
<api-endpoint openapi-path="../transactions.yaml" endpoint="/v0/transaction/{sender}/{receiver}" method="POST">
    <response type="200">
        <sample>
{
	"success": true,
	"message": {
		"id": "transaction_34210bja3421834jah6jhh3h67hd34j57bh24301",
		"sender": "AT10000000123456789012",
		"receiver": "AT10000000098765432112",
		"amount": "13.37",
		"description": Hello World,
		"created": "2024-01-12T11:32:40.579Z"
	}
}
        </sample>    
    </response>
    <response type="202">
        <sample>
{
    "success": false,
    "error": {
        "message": "There was an internal Server Error. Please try again later",
        "code": 500
    }
}
        </sample>
    </response>
</api-endpoint>

<!--<api-doc openapi-path="../transactions.yaml">
    
</api-doc>-->