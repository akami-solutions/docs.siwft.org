# Wallet Hub

<api-doc openapi-path="../hub.yaml">

<api-endpoint openapi-path="../hub.yaml" endpoint="/v0/hub/{hubID}" method="GET">
    <response type="200">
        <sample>
{
    "success": true,
    "message": {
        "name": "Your Hub Name",
        "domain": "https://domain.tld",
        "contact": "contact@domain.tld", // Null if no API Key entered
        "support": "support@domain.tld",
        "active": true,
        "apiKey": "api_52da990g5bdg0c829db34e8c57568557fg83c524", // Null if no API Key entered
        "created": "2024-01-12T11:32:40.579Z"
    }
}
        </sample>
    </response>
</api-endpoint>
<api-endpoint openapi-path="../hub.yaml" endpoint="/v0/hub/create" method="POST">
    <response type="200">
        <sample>
{
    "success": true,
    "message": {
        "name": "Your Hub Name",
        "domain": "https://domain.tld",
        "contact": "contact@domain.tld",
        "support": "support@domain.tld",
        "active": true,
        "apiKey": "api_52da990g5bdg0c829db34e8c57568557fg83c524",
        "created": "2024-01-12T11:32:40.579Z"
    }
}
        </sample>    
    </response>
</api-endpoint>