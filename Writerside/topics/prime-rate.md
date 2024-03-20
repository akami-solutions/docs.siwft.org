# Prime Rate

> **WARNING**
>
> This system has been around for a short time, so there may be changes and errors in the documentation.
{style="warning"}

Since March 15, 2024, SIWFT has a system called a "prime rate." This might sound complicated, but let's break it down!
## How does the prime rate work?

Imagine SIWFT as a giant piggy bank for digital money.  Wallet Hubs are like smaller piggy banks that connect to SIWFT.

The prime rate is like a special interest rate. Interest rates are basically rewards you get for saving or lending money. A higher interest rate means you get a bigger reward!

With the prime rate, SIWFT can control the flow of digital money in the system. This helps keep things balanced, kind of like how traffic lights control cars on the road. By adjusting the prime rate, SIWFT can:

*    Encourage saving: A higher prime rate might make Wallet Hubs offer better interest rates to their customers, making saving more attractive.
*    Control inflation: Inflation happens when things generally get more expensive over time. By adjusting the prime rate, SIWFT can try to slow down inflation and keep prices stable.
*    Influence exchange rates: Exchange rates determine how much of one digital currency you need to buy another. The prime rate can help keep exchange rates from changing too quickly.

The prime rate is an important tool for SIWFT, similar to how traffic lights are important for keeping traffic smooth!
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
