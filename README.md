# o-byter
AA exchange box for an address

Allows byte/asset exchange between owner and a un/known party

## How it works
Before first exchange, it has to be configured by setting: price to exchange, asset id, exchange direction and (optional) allowed address to exchange.

After that, unknown parties (or one only) can exchange until AA runs out of asset/byte.

Owner can deposit any amount or withdraw all bytes and defined asset anytime (sending `withdraw`= 1).

## How to configure
Send `configure` with value 1:

- Asset can be configured by sending an asset (will be sent back) or by setting it with `asset` param.

- Price -> `price` param. Expressed in bytes per one asset.

- Allowed address -> `address` param. Aditionally, it can be cleared sending `clear` as value.

- Exchange direction -> `want` param. Valid values: `asset` or `byte`.

## AA registration (https://github.com/jldevelops/o-waar)
Owner is able to register the AA so it could be used with @name instead of address.

To do so, send `register`=1 and `name` with desired name.
