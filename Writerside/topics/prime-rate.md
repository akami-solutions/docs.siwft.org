# Prime Rate

> **WARNING**
>
> This system has been around for a short time, so there may be changes and errors in the documentation.
{style="warning"}

Since 15.03.2024, SIWFT has had a prime rate system to which all wallet hubs must adhere.

## What is a prime rate?

The prime rate is a fixed interest rate at which the wallet hubs can borrow or invest money with the SIWFT. It is used to control the currency market, i.e. to influence the economic situation, inflation and the exchange rate of currencies, and is therefore one of the most important instruments of the SIWFT and the banking system of the real world.
[Source: n26.com](https://n26.com/de-de/blog/ezb-leitzins)

## How do I get the SIWFT prime rate?

In order to make it very easy for wallet hubs and individuals to query the SIWFT prime rate, you can query the SIWFT prime rate at any time without an API key or similar with the following request.

<api-endpoint openapi-path="../prime-rate.yaml" endpoint="/prime-rate" method="GET">
    <response type="200">
        <sample>
{
"value": 0
}
        </sample>    
    </response>
</api-endpoint>
