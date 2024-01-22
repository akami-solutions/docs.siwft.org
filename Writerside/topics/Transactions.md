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
> Please keep in mind that transactions over 10.000 needs to be Verified manually by SIWFT
> 
{style="note"}
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
>
> This endpoint was newly added on 22.01.2024
<api-endpoint openapi-path="../transactions.yaml" endpoint="/v0/transaction/" method="GET">
    <response type="200">
        <sample>
{
	"success": true,
	"message": [
		{
			"id": "transaction_114e5793868a8480411c73e3d45b6cd7cee8c012",
			"from": "AT10000000098765432112",
			"to": "AT10000000123456789012",
			"amount": "13.37",
			"message": "Hello World #1",
			"date": "2024-01-08T12:09:19.273Z",
			"holdBack": false
		},
		{
			"id": "transaction_a33e801d40225b99f34f988404f06259b3f98b82",
			"from": "AT10000000123456789012",
			"to": "AT10000000098765432112",
			"amount": "13.37",
			"message": "Hello World #2",
			"date": "2024-01-08T12:11:05.486Z",
			"holdBack": true
		}
	]
}
        </sample>
    </response>
</api-endpoint>
>
> This endpoint was newly added on 22.01.2024
<api-endpoint openapi-path="../transactions.yaml" endpoint="/v0/transaction/{transactionId}" method="GET">
    <response type="200">
        <sample>
{
	"success": true,
	"message":
		{
			"id": "transaction_114e5793868a8480411c73e3d45b6cd7cee8c012",
			"from": "AT10000000098765432112",
			"to": "AT10000000123456789012",
			"amount": "13.37",
			"message": "Hello World #1",
			"date": "2024-01-08T12:09:19.273Z",
			"holdBack": false
		}
}
        </sample>
    </response>
</api-endpoint>
