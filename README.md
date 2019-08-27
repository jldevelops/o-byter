# o-byter
AA exchange box for an address

Allows byte/asset exchange between owner and a un/known party

## How it works
Owner deposits amounts to exchange. Then, configures the exchange by setting: price to exchange, asset id, exchange direction and (optional) allowed address to exchange.

After that, unknown parties (or one only) can exchange until AA run out of asset/byte.

Owner can withdraw any amount anytime.

## How to configure
Send param "configure" with value 1:

- Asset can be configured by sending an asset (will be bounced back) or by setting it with "asset" param.

- Price is set with "price" param.

- Allowed address is set with "address" param. Aditionally, it can be cleared sending "clear" as value.

- Exchange direction: set it with "want" param. Valid values: "asset" or "byte".
