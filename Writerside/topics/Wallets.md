# Wallets
## Get a Wallet
> **WARNING**
> 
> SINCE THE 15.04.2024 RELEASE SERVER-SIDE CACHE IS ENABLED AND CAN LEAD TO OUTDATED OUTPUT. 
> 
>USE `Pragma:no-cache` HEADER TO PREVENT SERVER-SIDE CACHED DATA
{style="warning"}


<api-endpoint openapi-path="../wallet.yaml" endpoint="/v0/wallet/{walletID}" method="GET">
    <response type="200">
        <sample lang="JSON">
{
    "success": true,
    "message": {
        "username": "Your Username",
        "isActive": true,
        "isEnterprise": false,
        "balance": 13.37,
        "key": "key_h246375h24672510ffj8g3hh24678g2467dz4275"
    }
}
        </sample>
    </response>
</api-endpoint>
## Update a Wallets Username
> WARNING
> 
> New Since 15.04.2024
{style="note"}
<api-endpoint openapi-path="../wallet.yaml" endpoint="/v0/wallet/{walletID}" method="PATCH">
    <response type="200">
        <sample>
null
</sample>
</response>
</api-endpoint>
## Create a new Wallet

<api-endpoint openapi-path="../wallet.yaml" endpoint="/v0/wallet/create" method="POST">
    <response type="200">
        <sample>
{
	"success": true,
	"message": {
		"name": "Your Username",
		"country": "AT",
		"hubId": 10000000,
		"walletId": "1234567890",
		"walletPP": 61,
		"active": true,
		"balance": "13.37",
		"authKey": "key_h246375h24672510ffj8g3hh24678g2467dz4275"
	}
}
        </sample>
    </response>
</api-endpoint>
## Delete a Wallet
> WARNING
> 
> New Since 15.04.2024
{style="note"}
<api-endpoint openapi-path="../wallet.yaml" endpoint="/v0/wallet/{walletID}/delete" method="DELETE">
<response type="200">
<sample>
{
"success": true
}
</sample>
</response>
</api-endpoint>