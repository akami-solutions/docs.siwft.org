# Wallets

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
<api-endpoint openapi-path="../hub.yaml" endpoint="/v0/hub/create" method="POST">
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