# Account

accounts information

## Get Account Balances

```shell
https://public.xbts.io/account/getbalance/xbtsx
```
> The above command returns JSON all balances by account:

```json
[
  ......
  {
    "amount": 293000002,
    "asset": {
      "id": "1.3.4099",
      "symbol": "XBTSX.STH",
      "precision": 6,
      "issuer": "1.2.1003283",
      "options": {
        "max_supply": "200000000000000",
        "market_fee_percent": 0,
        "max_market_fee": 0,
        "issuer_permissions": 79,
        "flags": 4,
        "core_exchange_rate": {
          "base": {
            "amount": 100000,
            "asset_id": "1.3.0"
          },
          "quote": {
            "amount": 80000000,
            "asset_id": "1.3.4099"
          }
        },
        "whitelist_authorities": [

        ],
        "blacklist_authorities": [

        ],
        "whitelist_markets": [

        ],
        "blacklist_markets": [

        ],
        "description": "{\"main\":\"SmartHoldem - Decentralized Gaming Platform. Asset is backed 1:1 by the real STH on SmartHoldem blockchain https://smartholdem.io, and can be deposited and withdrawn using gateway https://xbts.io\",\"short_name\":\"STH\",\"market\":\"XBTSX.BTC\"}",
        "extensions": [

        ]
      },
      "dynamic_asset_data_id": "2.3.4099"
    }
  }
]
```

`GET https://public.xbts.io/account/getbalance/<AccountName>`

Return JSON information about all assets balances by account name.
