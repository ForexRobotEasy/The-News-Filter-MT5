# The News Filter MT5

The News Filter MT5 is an expert advisor developed by the Forex Robot Easy Team. It is a solution that filters expert advisors and charts based on news events in the Forex market. This code provides a sample implementation of the News Filter MT5.

## Features
- Filters expert advisors and manual charts during news time.
- Manages open positions and pending orders during news time.
- Connects to Forex Factory's economic calendar to determine news events.
- Customizable settings for maximum number of currency pairs and keywords.
- Gracefully exits the expert advisor after news time.

## How it Works
The expert advisor works by checking if it is news time. If it is, it filters the expert advisors and charts, manages open positions and pending orders, and then gracefully exits. The expert advisor connects to Forex Factory's economic calendar to determine if it is news time. It also uses a custom order management system to handle positions and orders.

## Usage
To use the News Filter MT5 expert advisor, follow these steps:
1. Import the necessary libraries: Trade, WebRequest, and ForexFactory.
2. Define the maximum number of currency pairs and keywords using the constants `MAX_CURRENCY_PAIRS` and `MAX_KEYWORDS`.
3. Initialize the order management system by calling the `InitializeOrderManagement()` function in the `OnInit()` function.
4. Connect to Forex Factory's economic calendar by calling the `ConnectToForexFactory()` function in the `OnInit()` function. If the connection fails, the expert advisor will print a message and return `INIT_FAILED`.
5. In the `OnTick()` function, check if it is news time by calling the `IsNewsTime()` function. If it is, filter the expert advisors and charts by calling the `FilterCharts()` function, manage open positions and pending orders by calling the `ManageOrders()` function, and then exit gracefully by calling the `ExpertRemove()` function.
6. Disconnect from Forex Factory's economic calendar by calling the `DisconnectFromForexFactory()` function in the `OnDeinit()` function.
7. Deinitialize the order management system by calling the `DeinitializeOrderManagement()` function in the `OnDeinit()` function.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample implementation and can work as described in the product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/news-filter-mt5-review-expert-advisor-and-chart-filtering-solution/).

## About Forex Robot Easy
Forex Robot Easy is a website that provides reviews and analysis of Forex trading robots and expert advisors. We aim to help traders make informed decisions by providing detailed information and trading results of various Forex products. For more information, please visit our [website](https://forexroboteasy.com/).
