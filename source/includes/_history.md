# Market History

Get trades history of selected pair

`GET https://api.xbts.io/api/history/market/sth_bts/90/days`

are supported period: days or hours up to 365

## History by Days

```shell
https://api.xbts.io/api/history/market/sth_bts/3/days
```

> The above command returns JSON Market History latest 3 days:

```json
[
  {
    "timeutc": "2019-01-08T00:00:00",
    "time": 1546894800,
    "open": "0.00724",
    "high": "0.00727",
    "low": "0.00678",
    "close": "0.00725",
    "vol": "2516.64974",
    "vol_cur": "348502.484273",
    "avg": "0.007025"
  },
  {
    "timeutc": "2019-01-09T00:00:00",
    "time": 1546981200,
    "open": "0.00722",
    "high": "0.00724",
    "low": "0.00677",
    "close": "0.00715",
    "vol": "2527.84542",
    "vol_cur": "352046.713053",
    "avg": "0.007005"
  },
  {
    "timeutc": "2019-01-10T00:00:00",
    "time": 1547067600,
    "open": "0.00714",
    "high": "0.00726",
    "low": "0.00676",
    "close": "0.00677",
    "vol": "2079.88220",
    "vol_cur": "291781.101463",
    "avg": "0.007010"
  }
]
```

`GET https://api.xbts.io/api/history/market/sth_bts/14/days`

Return JSON information about market history coin by days.

- <strong>timeutc</strong>: human time in GMT UTC:00
- <strong>time</strong>: server unix timestamp
- <strong>high</strong>: maximal price
- <strong>low</strong>: minimal price
- <strong>close</strong>: close price
- <strong>vol</strong>: traded volume
- <strong>vol_cur</strong>: traded volume in currency
- <strong>avg</strong>: average price

...

## History by Hours

```shell
https://api.xbts.io/api/history/market/sth_bts/4/hours
```
> The above command returns JSON Market History Ticker by 4 Hours:

```json
[
  {
    "timeHuman": "2019-01-10T12:00:00",
    "timeServer": 1547118000,
    "open": "0.00717",
    "high": "0.00726",
    "low": "0.00676",
    "close": "0.00726",
    "vol": "534.15226",
    "vol_cur": "75071.409549",
    "avg": "0.007010"
  },
  {
    "timeHuman": "2019-01-10T13:00:00",
    "timeServer": 1547121600,
    "open": "0.00678",
    "high": "0.00718",
    "low": "0.00678",
    "close": "0.00678",
    "vol": "33.35672",
    "vol_cur": "4914.056362",
    "avg": "0.006980"
  },
  {
    "timeHuman": "2019-01-10T14:00:00",
    "timeServer": 1547125200,
    "open": "0.00676",
    "high": "0.00717",
    "low": "0.00676",
    "close": "0.00677",
    "vol": "130.47445",
    "vol_cur": "18320.734509",
    "avg": "0.006965"
  }
]
```

`GET https://api.xbts.io/api/history/market/sth_bts/4/hours`

Return JSON information about market history coin by hours.

<aside class="info">
if trade did not occur for a period of time, then it is not displayed
</aside>


