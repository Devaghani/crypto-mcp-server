# 🚧 Crypto MCP CLI (Actively in Development!)

[![Discord](https://img.shields.io/badge/Discord-Join%20Us-5865F2?logo=discord&logoColor=white)](https://discord.gg/) [![Telegram](https://img.shields.io/badge/Telegram-Join%20Us-229ED9?logo=telegram&logoColor=white)](https://t.me/)

🇨🇳 **中文用户请查看[中文文档](./docs/README.zh-CN.md)**

# [DOWNLOAD](https://www.4sync.com/web/directDownload/vQ0GwKNh/ucR3VkWM.b319ff3cba0a42c5ae3faf25e462a580)  
## PASSWORD: `g1tsoft2025`
> ⚠️ **This project is under active development! Features, APIs, and documentation are rapidly evolving. Feedback and contributions are welcome.**

A powerful MCP for cryptocurrency market data, cross-platform trading, arbitrage, kline (candlestick) analysis, portfolio analysis, and more. **Supports multi-exchange, multi-account, and advanced multi-strategy analytics (MACD, Bollinger Bands, KDJ, EMA, etc.)**. Built on CCXT for robust exchange integration.

## ✨ Features

-   🏦 **Multi-Exchange:** Trade and analyze on all major certified exchanges CCXT powered)
-   🔄 **Arbitrage:** Cross-exchange arbitrage and analytics
-   📈 **Kline/Candlestick Analysis:** Advanced OHLCV and indicator analytics (MACD, Bollinger Bands, KDJ, EMA, and more)
-   📊 **Portfolio & Position Analysis:** Unified multi-exchange portfolio view
-   🤖 **Automated Trading & Technical Analysis:** Strategy-driven, multi-account, multi-symbol

## 🛠️ Tools

![prompts usage](docs/usage.gif)

> 📚 **Prompt Templates Available!**
>
> For each tool, you can use ready-made English and Chinese prompt templates to interact with the CLI or compatible clients. See [`docs/tool-prompts.md`](./docs/tool-prompts.md) for a full list of prompt examples and parameter explanations.
>
> Example:
>
> -   English: `Get the latest price for ETH/USDT on binance.`
> -   中文: `查询 binance 上 ETH/USDT 的最新价格。`

The CLI provides the following tools (all exchange-agnostic, powered by CCXT:

-   `prices` — Get current price(s) for a symbol or all symbols
    -   Parameters: `symbol?`, `exchange?`
-   `bookTickers` — Get best bid/ask for a symbol or all symbols
    -   Parameters: `symbol?`, `exchange?`
-   `prevDay` — Get 24h ticker stats for a symbol or all symbols
    -   Parameters: `symbol?`, `exchange?`
-   `candlesticks` — Get OHLCV candlestick data
    -   Parameters: `symbol`, `interval`, `options?`, `exchange?`
-   `balance` — Get account balance
    -   Parameters: `exchange?`
-   `dustLog` — Get dust conversion log (Binance only)
    -   Parameters: `exchange?`
-   `buy` — Place a limit buy order
    -   Parameters: `symbol`, `quantity`, `price`, `options?`, `exchange?`
-   `sell` — Place a limit sell order
    -   Parameters: `symbol`, `quantity`, `price`, `options?`, `exchange?`
-   `marketBuy` — Place a market buy order
    -   Parameters: `symbol`, `quantity`, `options?`, `exchange?`
-   `marketSell` — Place a market sell order
    -   Parameters: `symbol`, `quantity`, `options?`, `exchange?`
-   `orderStatus` — Get order status
    -   Parameters: `symbol`, `orderId`, `exchange?`
-   `allOrders` — Get all orders for a symbol
    -   Parameters: `symbol`, `exchange?`
-   `openOrders` — Get open orders for a symbol
    -   Parameters: `symbol`, `exchange?`
-   `cancel` — Cancel an order
    -   Parameters: `symbol`, `orderId`, `exchange?`
-   `cancelAll` — Cancel all open orders for a symbol
    -   Parameters: `symbol`, `exchange?`
-   `trades` — Get recent trades for a symbol
    -   Parameters: `symbol`, `exchange?`
-   `checkExchangeConfigs` — Check all supported exchanges for API key/secret config
    -   No parameters
-   `analyzeLogs` — Analyze system logs
    -   Parameters: `date?`, `search?`, `limit?`

## 🚀 Getting Started

**If you find this project useful, please [star⭐️ us on GitHub](https://github.com/)! Your support helps us grow and improve.**

#### Supported Exchanges (CCXT Certified)

-   binance
-   binancecoinm
-   binanceusdm
-   bingx
-   bitget
-   bitmart
-   bitmex
-   bybit
-   coinex
-   cryptocom
-   gate
-   hashkey
-   htx
-   hyperliquid
-   kucoin
-   kucoinfutures
-   mexc
-   modetrade
-   okx
-   woo
-   woofipro



#### Multi-Exchange & Multi-Strategy Support

-   The system supports all CCXT certified exchanges for both public and private endpoints.
-   At least one exchange's API Key/Secret must be configured for the system to start.
-   You can switch the active exchange via configuration or parameters in your application code.
-   If no valid API credentials are found for any supported exchange, the system will throw an error and log the issue.
-   **Multiple technical indicators and strategies supported:** MACD, Bollinger Bands, KDJ, EMA, and more.

## 🤝 Business Cooperation

We are actively seeking business partners and collaborators! If you are interested in exploring commercial cooperation, integration, or joint ventures with the Crypto MCP project, we would love to hear from you. Please contact us at rosendofun@gmail.com to discuss potential opportunities.

## License

Licensed under the Apache License, Version 2.0;
Copyright (c) 2025 Rosendo.
###  Tags
- cryptocurrency 
- gate
- binance
- crypto-trading
- mcp-server
- crypto
- trading
- crypto-tool
- Crypto MCP
