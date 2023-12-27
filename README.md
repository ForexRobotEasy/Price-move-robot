# Price Move Robot

This code is an example of a trading robot developed in MQL5 language. It is designed to execute trades based on the movement of prices and the RSI (Relative Strength Index) indicator. The robot opens buy trades when the RSI is below 30, indicating an oversold condition, and sells trades when the RSI is above 70, indicating an overbought condition.

## Input Parameters

- `StopLossPercent`: Stop loss percentage for the trades.
- `PeriodRSI`: RSI period for the indicator.
- `TrailingStop`: Trailing stop level for the trades.

## Global Variables

- `stopLossLevel`: Stop loss level calculated based on the input parameters.
- `takeProfitLevel`: Take profit level calculated based on the input parameters.
- `ticket`: Trade ticket number to keep track of the existing trade.

## Expert Initialization Function

The `OnInit()` function is called during the initialization of the expert advisor. In this function, the stop loss and take profit levels are calculated based on the input parameters.

## Expert Tick Function

The `OnTick()` function is called on each tick of the price data. It checks if there is an existing trade and if not, it checks the RSI value to determine whether to open a buy or sell trade. If there is an existing trade, it checks if the current trade is in profit and adjusts the stop loss level using a trailing stop.

## Expert Deinitialization Function

The `OnDeinit()` function is called when the expert advisor is being shut down. In this function, the existing trade is closed if there is one.

## Custom Functions

The `NormalizeDouble()` function is a custom function used to round a double value to a specified number of digits.

Please note that this code is provided as a sample and is not the official product. The official developer of this product can be found by using MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/price-move-robot-review-efficient-forex-software-for-optimal-trades/). ForexRobotEasy is not the official developer of this product, but they provide information and reviews on various Forex robots.
