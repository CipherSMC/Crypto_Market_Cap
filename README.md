# Crypto Market Cap & Token Analysis (Pine Script® v6)

A versatile TradingView indicator designed to track and visualize the Market Capitalization of the entire crypto market or specific tokens directly on your chart. This tool bridges the gap between price analysis and fundamental market-wide data.

## 🚀 Features

- **Global Market Overview**: Quickly toggle between:
  - **TOTAL**: Total Crypto Market Cap.
  - **TOTAL2**: Total Market Cap excluding Bitcoin (Altcoin Market).
  - **TOTAL3**: Total Market Cap excluding Bitcoin and Ethereum.
  - **OTHERS**: Market Cap of the rest of the market (excluding the Top 10 assets).
- **Dynamic Token Market Cap**: Select the "Current Asset" mode to automatically fetch the market cap for the token you are currently viewing (e.g., viewing `SOLUSDT` will display `CRYPTOCAP:SOL`).
- **Smart Formatting**: Values are automatically formatted into Trillions (T), Billions (B), or Millions (M) for clear readability.
- **Visual Trends**: Features a color-coded area plot with a vertical gradient, changing colors based on positive or negative market cap momentum.
- **Error Handling**: Built-in detection for assets that do not yet have an official `CRYPTOCAP` ticker on TradingView.

## 🛠️ How It Works

The indicator uses the `request.security()` function to pull data from the `CRYPTOCAP` data provider. When the "Current Asset" mode is enabled, it extracts the base currency from the current symbol (e.g., `BTC` from `BTC/USDT`) and constructs the appropriate ticker string.

## 📋 Settings

- **Market Cap Type**: Choose between Global aggregates or the "Current Asset".
- **Up/Down Colors**: Customize the visual appearance of the trend.
- **Tooltips**: Hover over the settings in the UI for detailed explanations of each market cap category.

## 📄 License

This Pine Script® code is subject to the terms of the Mozilla Public License 2.0 at https://mozilla.org/MPL/2.0/

---
*Disclaimer: This tool is for educational and informational purposes only. Market data is provided by TradingView's CRYPTOCAP database.*
