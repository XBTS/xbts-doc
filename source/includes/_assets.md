# Assets

Total information about XBTS coins
Since several exchanges operate in the blockchain, all XBTS-coins have a unique internal prefix - XBTSX.X

- X: coin such as WAVES, BTC, STH etc.

## List Available Assets on XBTS exchange.

```shell
https://api.xbts.io/api/assets
```
> The above command returns JSON all balances by account:

```json
[
  {
      "ticker": "BTC",
      "title": "Bitcoin",
      "precision": 8,
      "market_fee_percent": 0.05,
      "market_supply": 1.258605,
      "type": "coin",
      "id": "4157",
      "issuer": "1.2.1014725",
      "prefix": "XBTSX",
      "website": "https://bitcoin.org",
      "explorer": "https://blockexplorer.com"
  },
  {
        "ticker": "COF",
        "title": "CoffeeCoin",
        "precision": 3,
        "market_fee_percent": 0.05,
        "market_supply": 602354.514,
        "type": "token_waves",
        "id": "4581",
        "issuer": "1.2.1106976",
        "prefix": "XBTSX",
        "website": "https://wavesplatform.com/",
        "explorer": "http://wavesexplorer.com/"
  },
  {
      "ticker": "STH",
      "title": "SmartHoldem",
      "precision": 6,
      "market_fee_percent": 0,
      "market_supply": 36557779.092862,
      "type": "coin",
      "id": "4099",
      "issuer": "1.2.1003283",
      "prefix": "XBTSX",
      "website": "https://smartholdem.io",
      "explorer": "https://blockexplorer.smartholdem.io"
  }
    ...
```

`GET https://api.xbts.io/api/assets`

- <strong>market_fee_percent:</strong> trade percent
- <strong>market_supply:</strong> how many real coins are issued in XBTS, updated every 15-30 minutes
- <strong>type</strong>: coin, token_waves or token_eth
- <strong>id</strong>: internal asset id in blockchain
- <strong>issuer</strong>: issuer id in blockchain
- <strong>prefix</strong>: internal asset prefix in blockchain, example for XBTS exchange https://ex.xbts.io/#/asset/XBTSX.BTC

Return JSON information about all XBTS assets.
