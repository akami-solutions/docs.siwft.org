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

<api-doc openapi-path="../transactions.yaml"></api-doc>