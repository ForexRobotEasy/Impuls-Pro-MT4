# Impuls Pro MT4

**Developer: Forex Robot Easy Team**  
**Developer's site: [forexroboteasy.com](https://forexroboteasy.com)**

This code is an expert advisor for MetaTrader 4 platform that implements a swing trading strategy based on the iPump indicator. The expert advisor trades on the specified symbol and timeframe using predefined lot size, stop loss, and take profit levels.

## Strategy

The expert advisor uses the iPump indicator to identify sharp impulses in the market. The iPump indicator calculates the impulses based on the closing prices. The strategy is as follows:

1. Initialize the expert advisor by setting the trade parameters and creating the iPump indicator.
2. On each tick, calculate the impulse using the iPump indicator and get the current market price.
3. If the impulse is negative and the current price is higher than the overbought level of the iPump indicator, enter a buy trade with the specified lot size, stop loss, and take profit.
4. If the impulse is positive and the current price is lower than the oversold level of the iPump indicator, enter a sell trade with the specified lot size, stop loss, and take profit.
5. Perform necessary cleanup before deinitializing the expert advisor by deleting the iPump indicator.

## Usage

To use this expert advisor, follow these steps:

1. Include the necessary libraries: `Trade.mqh` and `iPump.mqh`.
2. Define the constants for lot size, stop loss, and take profit.
3. Initialize the global variables: `trade` and `iPump`.
4. Implement the `OnInit()` function to set the trade parameters and initialize the iPump indicator.
5. Implement the `OnTick()` function to execute trades based on the swing trading strategy and iPump indicator.
6. Implement the `OnDeinit()` function to perform necessary cleanup before deinitializing the expert advisor.
7. Optionally, implement the `TestEA()` function to test the expert advisor in different market conditions.

## Disclaimer

This code is provided as a sample implementation of the Impuls Pro MT4 expert advisor. Forex Robot Easy is not the official developer of this product. For detailed reviews and trading results of this product, please visit the official developer's website: [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-impuls-pro-mt4-a-professional-forex-traders-perspective/). To find the official developer of this product, please use MQL5.
