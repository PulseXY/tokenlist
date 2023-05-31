# PulseXY Tokenlist

## Adding Your Token
1. Add an entry in the `tokens` field of the appropriate tokenlist. Here is an example using WPLS:
    ```json
    {
      "name": "Wrapped PLS",
      "symbol": "WPLS",
      "chainId": 369,
      "decimals": 18,
      "address": "0xA1077a294dDE1B09bB078844df40758a5D0f9a27",
      "logoURI": "https://pulsexy.io/images/tokens/0xA1077a294dDE1B09bB078844df40758a5D0f9a27.png"
    }
    ```
2. Update the `timestamp` field to the current timestamp.
3. Update the `version` field to adhere to semantic versioning:

    * Increment major version when tokens are removed
    * Increment minor version when tokens are added
    * Increment patch version when tokens already on the list have minor details changed (name, symbol, logo URL, decimals)

    ***Note:*** Changing a token address or chain ID is considered both a remove and an add, and should be a major version update.
