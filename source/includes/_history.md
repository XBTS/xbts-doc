#Trade History

`GET https://public.xbts.io/history/<STEP>/<QUOTE_COIN>/<BASE_COIN>/<LIMIT>/<ToTimeStamp>`

STEP = day or hour

## History by Days

```shell
https://public.xbts.io/history/day/STH/BTS/7/1534293135
```
> The above command returns JSON Trade History 7 days (week) / Step 1 day:

```json

  "Response": "Success",
  "Data": [
    {
      "time": 1533765600,
      "humanTime": "2018-08-09T00:00:00",
      "high": "0.03200",
      "low": "0.02002",
      "open": "0.02500",
      "volumefrom": "204872.71448",
      "volumeto": "5769.16014",
      "close": "0.029613"
    },
    {
      "time": 1533852000,
      "humanTime": "2018-08-10T00:00:00",
      "high": "0.02961",
      "low": "0.02164",
      "open": "0.02960",
      "volumefrom": "169364.04439",
      "volumeto": "4110.76956",
      "close": "0.028679"
    },
 .....
    {
      "time": 1534284000,
      "humanTime": "2018-08-15T00:00:00",
      "high": "0.03601",
      "low": "0.03601",
      "open": "0.03601",
      "volumefrom": "8.19994",
      "volumeto": "0.29532",
      "close": "0.036015"
    }
  ],
  "TimeTo": "1534293135"
}
```

`GET https://public.xbts.io/history/day/<QUOTE_COIN>/<BASE_COIN>/<LIMIT>/<ToTimeStamp>`

Return JSON information about history coin by days.

Support XBTSX coins:

- STH
- BTC
- DOGE
- LTC
...

## History by Hours

```shell
https://public.xbts.io/history/hour/STH/BTS/24/1534293135
```
> The above command returns JSON Trade History 24 Hours/ Step 1 hour:

```json

  "Response": "Success",
  "Data": [
{
      "time": 1534201200,
      "humanTime": "2018-08-14T01:00:00",
      "high": "0.03990",
      "low": "0.03890",
      "open": "0.03890",
      "volumefrom": "9399.29474",
      "volumeto": "370.77409",
      "close": "0.039900"
    },
    {
      "time": 1534204800,
      "humanTime": "2018-08-14T02:00:00",
      "high": "0.03747",
      "low": "0.02645",
      "open": "0.03523",
      "volumefrom": "41691.57997",
      "volumeto": "1291.86200",
      "close": "0.030088"
    },
   .........
    {
      "time": 1534284000,
      "humanTime": "2018-08-15T00:00:00",
      "high": "0.03601",
      "low": "0.03601",
      "open": "0.03601",
      "volumefrom": "8.19994",
      "volumeto": "0.29532",
      "close": "0.036015"
    }
  ],
  "TimeTo": "1534293135"
}
```

`GET https://public.xbts.io/history/hour/<QUOTE_COIN>/<BASE_COIN>/<LIMIT>/<ToTimeStamp>`

Return JSON information about history coin by hours.

Support XBTSX coins:

- STH
- BTC
- DOGE
- LTC
...

