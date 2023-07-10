# Bitcoin Futures Liquidation Price

When trading Bitcoin Futures Contracts, the allocated funds are used as collateral by the Exchange Platform in order to be able to open a position based on the desired leverage. If the asset's price moves against the position side strongly, past the liquidation price, The position is closed automatically and as a result, the collateral is used to pay the lenders and cover fees.

### Formula

The formula for calculating the liquidation price for a margin trade using currency "i" is as follows:

Here, "i" represents the currency "i", "Ai" represents the total amount of "i" assets, "Li" represents the borrowed amount of "x" asset, "Ri" represents the amount of interest payable on "x" asset, "Pi" represents the index price of the "x" asset/BTC (or USDT) pair, and finally "li" represents the liquidation price for "x" asset.

Liquidation is triggered when the risk ratio reaches the liquidation risk ratio .

Risk ratio = Total assets / (Total amount borrowed + Interest payable). Using the "i" currency as an example:

<img src="https://github.com/jesusgraterol/BitcoinFuturesLiquidationPrice/assets/136823357/46a63d24-1339-4f52-97a8-cb6fa73b61a2" width="500" height="200">

Therefore, the liquidation reference price for "i" currency is:

<img src="https://github.com/jesusgraterol/BitcoinFuturesLiquidationPrice/assets/136823357/27d11a4f-4418-415d-a97d-60b1ac5ca124" width="550" height="200">

Ratio of the index price to the liquidation reference price = (Liquidation price - Index price) / Index price.

[View Notebook](./bitcoinfuturesliquidationprice.ipynb)
