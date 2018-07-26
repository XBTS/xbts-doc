# Tickers

## Get Single Ticker

```shell
https://public.xbts.io/ticker/BTS_STH
```
> The above command returns JSON structured like this:

```json
{
  "BTS_STH": {
    "time": "2018-07-26T20:54:30",
    "base": "BTS",
    "quote": "STH",
    "latest": "0.01862000",
    "lowest_ask": "0.01860000",
    "highest_bid": "0.01615782",
    "percent_change": "-4.31",
    "base_volume": "1554.69051",
    "quote_volume": "83492.478995"
  }
}
```

`GET https://public.xbts.io/ticker/<ticker_pair>`

Return JSON.

## Get Custom Tickers

```shell
https://public.xbts.io/ticker/BTS_STH,BTS_BTC
```
> The above command returns JSON structured like this:

```json
{
  "BTS_STH": {
    "time": "2018-07-26T21:03:42",
    "base": "BTS",
    "quote": "STH",
    "latest": "0.01862000",
    "lowest_ask": "0.01860000",
    "highest_bid": "0.01615782",
    "percent_change": "-4.31",
    "base_volume": "1554.69051",
    "quote_volume": "83492.478995"
  },
  "BTS_CNY": {
    "time": "2018-07-26T21:03:42",
    "base": "BTS",
    "quote": "CNY",
    "latest": "0.71681813",
    "lowest_ask": "0.71692375",
    "highest_bid": "0.71684642",
    "percent_change": "1.15",
    "base_volume": "11306693.30177",
    "quote_volume": "16018329.0389"
  }
}
```

`GET https://public.xbts.io/ticker/<ticker_pair1>,<ticker_pair2>,<ticker_pairN>`

<strong>List the pairs by separating them with commas</strong>

## Get All XBTS Tickers
```shell
https://public.xbts.io/tickers
```
> The above command returns JSON structured like this:

```json
{
  "BTS_STH": {
    "time": "2018-07-26T21:05:21",
    "base": "BTS",
    "quote": "STH",
    "latest": "0.01862000",
    "lowest_ask": "0.01860000",
    "highest_bid": "0.01615782",
    "percent_change": "-4.31",
    "base_volume": "1554.69051",
    "quote_volume": "83492.478995"
  },
  "BTS_POST": {
    "time": "2018-07-26T21:05:21",
    "base": "BTS",
    "quote": "POST",
    "latest": "0.06500000",
    "lowest_ask": "0.11999987",
    "highest_bid": "0.06500000",
    "percent_change": "0",
    "base_volume": "0",
    "quote_volume": "0"
  },
  "BTS_DOGE": {
    "time": "2018-07-26T21:05:21",
    "base": "BTS",
    "quote": "DOGE",
    "latest": "0.00874400",
    "lowest_ask": "0.00000000",
    "highest_bid": "0.00000000",
    "percent_change": "0",
    "base_volume": "0",
    "quote_volume": "0"
  },
  ....
}
```

`https://public.xbts.io/tickers`

<strong>Default base ticker BTS</strong>

## Get Custom Base Tickers
```shell
https://public.xbts.io/tickers?coin=BTC
```
> The above command returns JSON structured like this:

```json
{
  "BTC_STH": {
    "time": "2018-07-26T21:09:27",
    "base": "BTC",
    "quote": "STH",
    "latest": "0.00000050",
    "lowest_ask": "0.00000050",
    "highest_bid": "0.00000042",
    "percent_change": "0.35",
    "base_volume": "0.04553569",
    "quote_volume": "98815.095234"
  },
  "BTC_POST": {
    "time": "2018-07-26T21:09:27",
    "base": "BTC",
    "quote": "POST",
    "latest": "0.00000198",
    "lowest_ask": "0.00000205",
    "highest_bid": "0.00000170",
    "percent_change": "-3.41",
    "base_volume": "0.03290543",
    "quote_volume": "16515.795701"
  },
  "BTC_DOGE": {
    "time": "2018-07-26T21:09:27",
    "base": "BTC",
    "quote": "DOGE",
    "latest": "0.00000042",
    "lowest_ask": "0.00000046",
    "highest_bid": "0.00000042",
    "percent_change": "0",
    "base_volume": "0.00254446",
    "quote_volume": "6058.26082"
  },
  ....
}
```

`https://public.xbts.io/tickers?coin=<BASE_COIN>`

<strong>Default base ticker BTS</strong>