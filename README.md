## ReadMe - Evening Scalper Pro MT5

This is a ReadMe file for the code of the Evening Scalper Pro MT5 expert advisor. Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in the product. To find the official developer of this product, please use MQL5.

### Product Description

Evening Scalper Pro MT5 is a state-of-the-art mean reversion trading system developed by the Forex Robot Easy Team. It is designed to trade multiple currency pairs during specific trading sessions, utilizing a unique trading logic.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Evening Scalper Pro MT5](https://forexroboteasy.com/forex-robot-review/review-evening-scalper-pro-mt5-a-state-of-the-art-mean-reversion-trading-system/).

### Usage Instructions

1. Define the currency pairs to be traded by modifying the `currencyPairs` array in the code. The provided array contains a list of example currency pairs.
2. Specify the trading session by setting the `startHour` and `endHour` variables. The expert advisor will only trade within this time frame.
3. Define the rollover hours to be avoided by setting the `rolloverStartHour` and `rolloverEndHour` variables. The expert advisor will not trade during this period.
4. Implement the unique trading logic by adding code to the `tradeLogic()` function. This is where you can customize the trading strategy according to your preferences.
5. If needed, modify the `enterMarketOrder()` and `exitMarketOrder()` functions to enter and exit market orders as per your broker's requirements.

### Custom Trading Functions

The code provides the following custom trading functions:

1. `isInSession()`: Checks if the current time is within the specified trading session.
2. `isRollover()`: Checks if the current time is within the rollover period.
3. `enterMarketOrder(symbol, type, volume)`: Enters a market order for the specified symbol, order type, and volume.
4. `exitMarketOrder(symbol)`: Exits a market order for the specified symbol.
5. `tradeLogic()`: Implements the unique trading logic. This is where you can define your trading strategy.

### Expert Advisor Start Function

The expert advisor's start function is `OnTick()`. It performs the following actions:

1. Checks if the current time is within the trading session. If not, it exits the function.
2. Checks if the current time is within the rollover period. If yes, it exits the function.
3. Implements the trading logic by calling the `tradeLogic()` function.

Please note that the expert advisor will only execute trades during the specified trading session and avoid trading during the rollover period.

For further information and support, please visit the [Forex Robot Easy](https://forexroboteasy.com/) website.
