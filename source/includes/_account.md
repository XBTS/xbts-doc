# Account

<strong>Information about accounts is public and is provided by the blockchain.</strong>

Displays balances that are not in orders

## Get Account Balances

```shell
https://public.xbts.io/account/getbalance/xbtsx
```
> The above command returns JSON all balances by account:

```json
{
  "BTS": "212.69768",
  "OPEN.DOGE": "0.0000",
  "DEEX": "0.1000",
  "PROTON": "0.0005",
  "ELECTRON": "1.0000",
  "NEXTCOIN": "0.0005",
  "VIRTUAL": "1.000",
  "CUBED.CNY": "0.000002",
  "XBTSX": "0.000000",
  "XBTSX.POST": "0.000000",
  "XBTSX.STH": "293.000002",
  "CUBED.USD": "0.000002"
}
```

`GET https://public.xbts.io/account/getbalance/<AccountName>`

Return JSON information about all assets balances by account name.

if not found account, return null:
