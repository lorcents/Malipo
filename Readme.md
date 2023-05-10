# MALIPO
local Payment gateway
####  3rd Party Apis

Daraja API
   >Mpesa Daraja Api.Consumed end point Mpesa express

Jenga API
  >Send Money with Equity Bank,Send to local banks with pesalink ,Send money to international with SWIFT,send money locally with RTGS,send money with local mobile providers.

Airtel Money
>Send and receive money with airtel

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/join-team?invite_code=edfd665f474f383ee545a161c1485a99&target_code=12291a4f448a2e2fd97751a7c36299f9)

## MPS Transaction

```mermaid
sequenceDiagram
UI->> VW: mps transaction
VW-->>MPS: stk push
VW-->> DB: seed transaction and logs
MPS-->> VW: mps callBack
VW ->>UI :Trasanction success
```

## Jenga Transaction
```mermaid
sequenceDiagram
UI->> VW: Jenga transaction
VW-->>JENGA: Jenga Request
VW-->> DB: seed transaction and logs
JENGA-->> VW: Jenga Response
VW ->>UI :Trasanction success
```
