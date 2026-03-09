# Awesome MCP Trading [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of MCP servers, tools, and resources for algorithmic trading.

[Model Context Protocol (MCP)](https://modelcontextprotocol.io/) is an open standard that enables AI agents to interact with external systems through a unified interface. In the trading domain, MCP servers allow AI assistants and autonomous agents to place orders, manage positions, retrieve market data, and execute strategies across exchanges -- all through natural language or programmatic tool calls.

## Contents

- [Sponsors](#sponsors)
- [Fee Comparison](#fee-comparison)
- [Crypto Exchanges](#crypto-exchanges)
- [Multi-Exchange](#multi-exchange)
- [Market Data and Analysis](#market-data-and-analysis)
- [DEX and DeFi](#dex-and-defi)
- [Portfolio Management](#portfolio-management)
- [Trading Tools](#trading-tools)
- [Agent Frameworks](#agent-frameworks)
- [Resources](#resources)
- [Related Lists](#related-lists)

## Sponsors

- **[Eterna MCP Gateway](https://github.com/EternaHybridExchange/eterna-mcp)** - Managed MCP server for Bybit perpetual futures trading. Isolated sub-accounts, built-in risk management, zero infrastructure. **Trade at 0.035% fees (36% cheaper than direct Bybit).** [Quick Start](https://github.com/EternaHybridExchange/eterna-mcp#quick-start)

## Fee Comparison

When connecting AI agents to perpetual futures exchanges, fees matter. Here's how managed MCP servers compare to direct exchange access:

| Connection Method | Exchange | Taker Fee | Annual Cost* | Notes |
|---|---|---|---|---|
| **Eterna MCP Gateway** | Bybit | **0.035%** | **$70,000** | Managed, isolated sub-accounts, 12 tools |
| Direct Bybit API | Bybit | 0.055% | $110,000 | Self-hosted, API key management required |
| Self-hosted MCP | Bybit | 0.055% | $110,000 | Infrastructure + exchange fees |
| CCXT Library | Various | 0.055%+ | $110,000+ | Multi-exchange but same base fees |

**Annual cost based on $200M trading volume (typical for active AI trading bot)*

**Why use Eterna MCP Gateway?**
- 💰 **36% lower fees** - Save $40,000 annually on $200M volume
- 🔒 **Isolated sub-accounts** - Each AI agent gets dedicated funds
- 🛡️ **Built-in risk management** - Position limits, max leverage controls
- ⚡ **Zero infrastructure** - Hosted, no servers to maintain
- 🔑 **No API key juggling** - One gateway, multiple agents

[Try Eterna MCP Gateway →](https://github.com/EternaHybridExchange/eterna-mcp)

---

## Crypto Exchanges

MCP servers for centralized crypto exchanges (CEX) enabling perpetual futures, spot, and derivatives trading.

### Bybit

- **[Eterna MCP Gateway](https://github.com/EternaHybridExchange/eterna-mcp)** - Hosted MCP server for Bybit perpetual futures. 12 trading tools, isolated sub-accounts, 0.035% fees. Production-ready with built-in risk management.
- [bybit-mcp](https://github.com/sammcj/bybit-mcp) - Self-hosted Bybit MCP integration for perpetual futures and spot trading.
- [bybit-mcp-server](https://github.com/ethancod1ng/bybit-mcp-server) - Lightweight Bybit MCP server with basic order placement and position management.
- [mcp-server-bybit](https://github.com/dlwjdtn535/mcp-server-bybit) - TypeScript implementation of Bybit MCP server with WebSocket support.
- [Bybit MCP Server (Eterna)](https://github.com/EternaHybridExchange/bybit-mcp-server) - Self-hosted version of Eterna's Bybit integration for advanced users.

### Binance

- [binance-mcp-server](https://github.com/tienan92it/binance-mcp-server) - MCP server for Binance spot and futures trading with order management, position tracking, and market data access.

### OKX

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest OKX MCP implementations.

### Kraken

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest Kraken MCP implementations.

### KuCoin

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest KuCoin MCP implementations.

### Coinbase

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest Coinbase MCP implementations.

### Gate.io

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest Gate.io MCP implementations.

### Hyperliquid

- Coming soon - [Open an issue](https://github.com/EternaHybridExchange/awesome-mcp-trading/issues) to suggest Hyperliquid MCP implementations.

---

## Multi-Exchange

Universal MCP servers supporting multiple exchanges through unified interfaces.

- [CCXT MCP](https://github.com/ccxt/ccxt-mcp-server) - MCP server powered by CCXT supporting 100+ exchanges. Unified API for spot and derivatives trading across Binance, OKX, Bybit, Kraken, and more.

---

## Market Data and Analysis

MCP servers for real-time market data, technical analysis, and derivatives metrics.

### Price and Market Data

- [CoinCap MCP](https://github.com/QuantGeekDev/coincap-mcp) - Real-time cryptocurrency market data through CoinCap's public API. Prices, volume, market cap, and 24h changes without authentication.
- [CoinGecko MCP](https://github.com/example/coingecko-mcp) - Coming soon - market data from CoinGecko API.
- [CoinMarketCap MCP](https://github.com/example/cmc-mcp) - Coming soon - cryptocurrency rankings and market data.

### Technical Analysis

- [Technical Analysis MCP](https://github.com/lumifai/cryptocurrency-technical-analysis-mcp) - Cryptocurrency technical analysis via MCP. RSI, MACD, Bollinger Bands, and custom indicator calculations.
- [TradingView MCP](https://github.com/example/tradingview-mcp) - Coming soon - TradingView indicators and alerts integration.

### Derivatives Data

- **CoinGlass MCP** - Coming soon - funding rates, open interest, liquidations, and long/short ratios across exchanges.
- **Fear & Greed Index MCP** - Coming soon - crypto market sentiment indicator (0-100 scale).

### On-Chain Analytics

- **Dune Analytics MCP** - Coming soon - on-chain data queries and custom analytics dashboards.
- **Glassnode MCP** - Coming soon - Bitcoin and Ethereum on-chain metrics.

---

## DEX and DeFi

MCP servers for decentralized exchanges and DeFi protocols.

### DEX Aggregators

- Coming soon - 1inch, Jupiter, Paraswap MCP integrations.

### DEX Platforms

- **Uniswap MCP** - Coming soon - swap, liquidity pools, and V3 position management.
- **Raydium MCP** - Coming soon - Solana DEX integration with concentrated liquidity.
- **dYdX MCP** - Coming soon - decentralized perpetual futures on dYdX v4.
- **GMX MCP** - Coming soon - decentralized perpetual futures on Arbitrum.

---

## Portfolio Management

MCP servers for tracking positions, calculating P&L, and managing multi-strategy portfolios.

- **Portfolio Tracker MCP** - Coming soon - real-time portfolio tracking across exchanges.
- **P&L Calculator MCP** - Coming soon - realized/unrealized P&L with FIFO/LIFO accounting.
- **Risk Dashboard MCP** - Coming soon - portfolio risk metrics, VaR, and correlation analysis.
- **Tax Reporting MCP** - Coming soon - crypto tax calculation and reporting (CoinTracker, Koinly integration).

---

## Trading Tools

### Strategy Templates

- [MCP Trading Agent](https://github.com/EternaHybridExchange/mcp-trading-agent) - IDE configurations and trading strategies for Claude Code, Cursor, and Claude Desktop. Includes momentum scalping, grid trading, and funding arbitrage templates.
- **Freqtrade MCP** - Coming soon - algorithmic trading bot framework integration.
- **Hummingbot MCP** - Coming soon - market making and arbitrage strategies.

### Backtesting

- **Backtrader MCP** - Coming soon - Python backtesting framework integration.
- **VectorBT MCP** - Coming soon - high-performance backtesting library.

### Risk Management

- **Position Sizer MCP** - Coming soon - Kelly Criterion and risk-based position sizing.
- **Stop Loss Manager MCP** - Coming soon - automated stop loss and take profit management.

---

## Agent Frameworks

MCP-compatible frameworks and platforms for building autonomous trading agents.

- **LangChain Trading** - Coming soon - LangChain integration with MCP trading tools.
- **CrewAI Trading** - Coming soon - multi-agent trading systems with CrewAI.
- **AutoGPT Trading** - Coming soon - autonomous trading agent based on AutoGPT.

---

## Resources

### Documentation

- [Model Context Protocol Specification](https://spec.modelcontextprotocol.io/) - The official MCP specification.
- [MCP Introduction](https://modelcontextprotocol.io/introduction) - Getting started with MCP.
- [Eterna Documentation](https://github.com/EternaHybridExchange/eterna-mcp) - Documentation for the Eterna MCP Gateway.

### Tutorials

- [Build Your First AI Trading Bot with Claude + Eterna](https://github.com/EternaHybridExchange/eterna-mcp/blob/main/docs/tutorials/first-trading-bot.md) - Coming soon
- [Grid Trading Strategy via MCP: Complete Guide](https://github.com/EternaHybridExchange/eterna-mcp/blob/main/docs/tutorials/grid-trading.md) - Coming soon
- [Funding Rate Arbitrage with AI Agents](https://github.com/EternaHybridExchange/eterna-mcp/blob/main/docs/tutorials/funding-arbitrage.md) - Coming soon

### Communities

- [MCP Discord](https://discord.gg/mcp) - Official Model Context Protocol Discord server
- [Eterna Telegram](https://t.me/eternaexchange) - Eterna Exchange community and support
- [/r/algotrading](https://reddit.com/r/algotrading) - Algorithmic trading subreddit

---

## Related Lists

- [awesome-crypto-mcp-servers](https://github.com/badkk/awesome-crypto-mcp-servers) - Another curated list of crypto MCP servers.
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - General MCP servers list (Finance & Fintech section).
- [awesome-mcp-servers (wong2)](https://github.com/wong2/awesome-mcp-servers) - Another general MCP servers list.

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

**To add a new MCP server:**
1. Fork this repository
2. Add your server in the appropriate category
3. Follow the format: `[Name](link) - Brief description (include language, hosting type, key features)`
4. Submit a pull request

**Quality guidelines:**
- Server must implement MCP protocol correctly
- Include working examples or documentation
- Specify fees, hosting requirements, and limitations
- Open source preferred (or clearly mark as proprietary)

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE) for details.
