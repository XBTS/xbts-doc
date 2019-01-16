# Tickers

<strong>You can get a list of XBTS tickers in any direction:</strong> sth_bts,sth_btc,sth_ruble,onion_egc

lowercase and uppercase tickers are supported: sth_bts,STH_BTC

## Get Single Ticker Pair

```shell
https://public.xbts.io/ticker/sth_bts
```
> The above command returns JSON structured like this:

```json
{
  "STH_BTS": {
    "high": "0.00726",
    "low": "0.006764",
    "avg": "0.00701",
    "vol": "2440.94632",
    "vol_cur": "342373.964876",
    "last": "0.00678",
    "buy": "0.00676",
    "sell": "0.00718",
    "percent_change": "-5.96",
    "updated": 1547125050
  }
}
```

<strong>Get current ticker information from blockchain</strong>

`GET https://public.xbts.io/ticker/sth_btc`

Return JSON.

- <strong>high</strong>: maximal price
- <strong>low</strong>: minimal price
- <strong>avg</strong>: average price
- <strong>vol</strong>: traded volume latest 24 hours
- <strong>vol_cur</strong>: traded volume in currency latest 24 hours
- <strong>last</strong>: last transaction price
- <strong>buy</strong>: buying price
- <strong>sell</strong>: selling price
- <strong>percent_change</strong>: percent change
- <strong>updated</strong>: last update from blockchain, GMT UTC:00

## Get Multi Tickers

<strong>List pairs separated by commas, without spaces</strong>

```shell
https://api.xbts.io/api/ticker/sth_bts,sth_waves,bts_btc,btc_ruble,nvc_btc
```
> The above command returns JSON structured like this:

```json
{
  "STH_BTS": {
    "high": "0.00726",
    "low": "0.006764",
    "avg": "0.00701",
    "vol": "2440.94632",
    "vol_cur": "342373.964876",
    "last": "0.00678",
    "buy": "0.00676",
    "sell": "0.00718",
    "percent_change": "-5.96",
    "updated": 1547125359
  },
  "BTS_BTC": {
    "high": "0.00001001",
    "low": "0.0000119",
    "avg": "0.00001095",
    "vol": "0.00510795",
    "vol_cur": "433.0283",
    "last": "0.00001011",
    "buy": "0.00001011",
    "sell": "0.00001189",
    "percent_change": "-15.07",
    "updated": 1547125359
  },
  "BTC_RUBLE": {
    "high": "273075.9148",
    "low": "273075.9148",
    "avg": "273075.9148",
    "vol": "0",
    "vol_cur": "0",
    "last": "273075.9148",
    "buy": "273075.9148",
    "sell": "300000",
    "percent_change": "0",
    "updated": 1547125359
  },
  ...
}
```

`GET https://api.xbts.io/api/ticker/sth_bts,sth_waves,bts_btc,btc_ruble,nvc_btc`

Return JSON

- <strong>high</strong>: maximal price
- <strong>low</strong>: minimal price
- <strong>avg</strong>: average price
- <strong>vol</strong>: traded volume latest 24 hours
- <strong>vol_cur</strong>: traded volume in currency latest 24 hours
- <strong>last</strong>: last transaction price
- <strong>buy</strong>: buying price
- <strong>sell</strong>: selling price
- <strong>percent_change</strong>: percent change
- <strong>updated</strong>: last update from blockchain, GMT UTC:00

## Liquid Pairs by Ticker

```shell
https://api.xbts.io/api/liquid/sth
```
> The above command returns JSON structured like this:

```json
{
  "pairs": {
...
    "STH_BTS": {
      "high": "0.00726",
      "low": "0.006764",
      "avg": "0.00701",
      "vol": "2559.83066",
      "vol_cur": "358982.717585",
      "last": "0.00717",
      "buy": "0.00676",
      "sell": "0.00718",
      "percent_change": "-0.55",
      "updated": 1547126883
    },
    "STH_BTC": {
      "high": "0.00000006",
      "low": "0.00000008",
      "avg": "0.00000007",
      "vol": "0.00046462",
      "vol_cur": "6738.041932",
      "last": "0.00000006",
      "buy": "0.00000005",
      "sell": "0.00000006",
      "percent_change": "-24.99",
      "updated": 1547126883
    },
    "STH_ONION": {
      "high": "0.00076923",
      "low": "0.00076923",
      "avg": "0.00076923",
      "vol": "8.63261094",
      "vol_cur": "11222.394222",
      "last": "0.00076923",
      "buy": "0.00076923",
      "sell": "0.00125",
      "percent_change": "15.38",
      "updated": 1547126883
    },
    "STH_ETH": {
      "high": "0.0000019",
      "low": "0.0000025",
      "avg": "0.0000022",
      "vol": "0.0011181",
      "vol_cur": "525.314441",
      "last": "0.0000025",
      "buy": "0.000002",
      "sell": "0.000003",
      "percent_change": "28.2",
      "updated": 1547126883
    },
    ...
  },
  "count": 15
}
```

<strong>Get current information about liquid ticker pairs from blockchain</strong>

`https://api.xbts.io/api/liquid/sth`

<strong>Returns a list of all pairs that were traded for the specified ticker in the last 24 hours</strong>

## Market 24h Tickers

```shell
https://api.xbts.io/api/market24
```
> The above command returns JSON structured like this:

```json
{
...
     "STH_BTS": {
      "high": "0.00692",
      "low": "0.00689",
      "avg": "0.0069",
      "vol": "2510.44111",
      "vol_cur": "365535.024925",
      "last": "0.00692",
      "buy": "0.00688",
      "sell": "0.00692",
      "percent_change": "-1.56",
      "updated": 1547589057
    },
    "BTC_BTS": {
      "high": "94786.72982",
      "low": "94786.72982",
      "avg": "94786.72982",
      "vol": "1278.91165",
      "vol_cur": "0.01351127",
      "last": "94786.72982",
      "buy": "84000.084",
      "sell": "94786.72982",
      "percent_change": "12.84",
      "updated": 1547589057
    },
    "WAVES_BTS": {
      "high": "72.5",
      "low": "72.5",
      "avg": "72.5",
      "vol": "0.07242",
      "vol_cur": "0.0009989",
      "last": "72.5",
      "buy": "72.5",
      "sell": "75",
      "percent_change": "0",
      "updated": 1547589057
    }
}
```

<strong>Get information about liquid market pairs in 24 hours</strong>

`https://api.xbts.io/api/market24`

- <strong>high</strong>: maximal price 24h
- <strong>low</strong>: minimal price 24h
- <strong>avg</strong>: average price 24h
- <strong>vol</strong>: traded volume latest 24 hours
- <strong>vol_cur</strong>: traded volume in currency latest 24 hours
- <strong>last</strong>: last transaction price
- <strong>buy</strong>: current buying price
- <strong>sell</strong>: current selling price
- <strong>percent_change</strong>: percent change 24h
- <strong>updated</strong>: last update from blockchain, GMT UTC:00

<strong>Returns a list of all pairs that were traded on market in the last 24 hours</strong>
