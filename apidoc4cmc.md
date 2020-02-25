**Get Summary**
----
  Returns exchange summary.

* **URL**

  /summary

* **Method:**

  `GET`
  
*  **URL Params**
  None

* **Response:**

  * **Code:** 200
    **Content:**
```{
  "success": true,
  "message": null,
  "dataVersion": "59b8474fbe293a34b5456ad15462a6e8b6a927e1",
  "data": {
    "btc_usd": {
      "last": "7296.0408661200",
      "percentChange": "0",
      "baseVolume": null,
      "quoteVolume": 0,
      "isFrozen": 1,
      "high24hr": "7296.0408661200",
      "low24hr": "7296.0408661200"
    }
  }
}
```

**Get Assets**
----
  Returns exchange assets.

* **URL**

  /assets

* **Method:**

  `GET`

* **Response:**

  * **Code:** 200
    **Content:**
```{
  "success": true,
  "message": null,
  "dataVersion": "59b8474fbe293a34b5456ad15462a6e8b6a927e1",
  "data": {
    "BTC": {
      "name": "Bitcoin",
      "unified_cryptoasset_id": 2001,
      "can_withdraw": true,
      "can_deposit": true,
      "min_withdraw": "3.0000000000",
      "max_withdraw": "10000.0000000000",
      "maker_fee": "0.0015",
      "taker_fee": "0.0015"
    }
  }
}
```


**Get Ticker**
----
  Returns exchange ticker.

* **URL**

  /ticker

* **Method:**

  `GET`

* **Response:**

  * **Code:** 200
    **Content:**
```{
  "success": true,
  "message": null,
  "dataVersion": "59b8474fbe293a34b5456ad15462a6e8b6a927e1",
  "data": {
    "BTC_USD": {
      "base_id": 0,
      "quote_id": 2001,
      "last_price": "7296.0408661200",
      "base_volume": 0,
      "quote_volume": null,
      "isFrozen": 1
    }
  }
}
```


**Get Market Trades**
----
  Returns market trades.

* **URL**

  /trades/[market_pair]

* **Method:**

  `GET`

* **Response:**

  * **Code:** 200
    **Content:**
```{
  "success": true,
  "message": null,
  "dataVersion": "59b8474fbe293a34b5456ad15462a6e8b6a927e1",
  "data": [
    {
      "trade_id": 7680481,
      "price": "9599.1200000000",
      "base_volume": "0.0010000000",
      "quote_volume": "9.5991200000",
      "trade_timestamp": 1582602285358,
      "type": "sell"
    }
  }
}
```



**Get Market Orderbook**
----
  Returns market orderbook.

* **URL**

  /orderbook/[market_pair]

* **Method:**

  `GET`

* **Response:**

  * **Code:** 200
    **Content:**
```{
  "success": true,
  "message": null,
  "dataVersion": "59b8474fbe293a34b5456ad15462a6e8b6a927e1",
  "data": {
    "bids": [
      [
        "0.0010000000",
        "9586.9100000000"
      ],
      [
        "0.0010000000",
        "9570.9500000000"
      ]
    ],
    "asks": [
      [
        "0.0010000000",
        "9587.9200000000"
      ],
      [
        "0.0010000000",
        "9603.8800000000"
      ],
    ],
  }
}
```

