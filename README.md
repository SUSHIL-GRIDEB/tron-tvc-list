# Adding new token
The JSON schema for the tokens includes: address, name, decimals, symbol, logoURI, official homepage, MarketCap link, existing Markets.

Follow the steps below to add a new token：
1) Fork this repo.
2) change the JSON file `tokenlist.json`, adding such as: (PLEASE DO NOT REMOVE EXISITING TOKENS)
```
{
      "address": "TGZEXC7y4mMpTMaTonXcGKH9iGoSxnukdx",
      "symbol": "KMH",
      "name": "KUMBH",
      "decimals": 18,
      "logoURI": "https://kumbh.co.in/image/maha_logo.png",
      "homepage": "https://kumbh.co.in/",
      "MarketCapLink": "https://coinmarketcap.com/currencies/kumbh/",
      "existingMarkets": [
          {
              "source": "Binance",
              "pairs": [
                  "KMH/USDT",
                  "KMH/BUSD",
                  "KMH/BNB",
                  "KMH/USDC"
              ]
          },
          {
              "source": "Poloniex",
              "pairs": [
                  "KMH/USDT"
              ]
          },
          {
              "source": "KuCoin",
              "pairs": [
                  "KMH/USDT"
              ]
          }
    ]
}
```
* `address`[Required]: your token address.
* `symbol`[Required]: your token symbol.
* `name`[Required]: your token name.
* `logoURI`[Required]: the logo URI of your token.
* `homepage`[Required]: the home page of your token.
* `MarketCapLink`[Optional]: the coinmarketcap or coingecko link for your token.
* `existingMarkets`[Required]: where to trade with your token.
3) Submit PR with the changed JSON file.


