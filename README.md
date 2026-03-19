# Antseer — The Web3 Data OS for the Agent Era

**[Website](https://antseer.ai)** · [中文](README.zh.md) · [日本語](README.ja.md) · [한국어](README.ko.md)

> One MCP endpoint. 100+ real-time Web3 data tools. Zero API keys required.

Antseer connects AI agents to live on-chain and market intelligence through a single [Model Context Protocol (MCP)](https://modelcontextprotocol.io) endpoint. Any MCP-compatible client auto-discovers all available tools on connection — no SDK, no configuration, no API keys.

---

## Quick Connect

**MCP Endpoint:** `https://ant-on-chain-mcp.antseer.ai/mcp`

### Claude Code

```bash
claude mcp add antseer --transport http https://ant-on-chain-mcp.antseer.ai/mcp
```

### Claude Desktop

Add to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "antseer": {
      "url": "https://ant-on-chain-mcp.antseer.ai/mcp",
      "transport": "http"
    }
  }
}
```

### Cursor / Windsurf

Add to your MCP settings:

```json
{
  "mcpServers": {
    "antseer": {
      "url": "https://ant-on-chain-mcp.antseer.ai/mcp",
      "transport": "http"
    }
  }
}
```

### OpenCode

```json
{
  "mcp": {
    "servers": {
      "antseer": {
        "url": "https://ant-on-chain-mcp.antseer.ai/mcp",
        "type": "http"
      }
    }
  }
}
```

---

## Data Categories

100+ tools across four domains, powered by multiple professional Web3 data providers.

### OnChain
- Protocol TVL, yields, fees & revenue tracking
- Smart money & whale wallet monitoring
- Cross-chain bridge fund flows
- Stablecoin market dynamics & supply analysis
- Meme token narrative detection & analytics
- Token on-chain metrics, holder distribution & PnL
- Wallet address profiling & counterparty analysis

### CeFi
- Spot market structure, pricing & order book depth
- Futures open interest, funding rates & liquidation tracking
- Market technical indicators
- Perpetual DEX analytics & whale position tracking

### TradFi
- Bitcoin & Ethereum ETF net inflows & AUM
- Tokenized US equities (price, history, OHLC)
- Tokenized precious metals

### Macro & Sentiment
- US macroeconomic indicators — GDP, CPI, Fed funds rate, Treasury yields, unemployment
- Crypto market sentiment scoring & social analytics

---

## Example Queries

Once connected, ask your AI agent naturally:

- *"Show me the top 10 DeFi protocols by TVL and their 7-day change"*
- *"What's the BTC funding rate across major exchanges right now?"*
- *"How much net inflow did Bitcoin ETFs receive this week?"*
- *"Which wallets are accumulating ETH in the last 24 hours?"*
- *"What's the current fear & greed index and market sentiment?"*

---

## CLI Tool

Antseer also provides a standalone CLI for direct data queries from your terminal.

→ See [cli.md](cli.md) for installation and usage.

**Quick install:**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows (PowerShell)
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

---

## Links

- **Website:** https://antseer.ai
- **MCP Endpoint:** https://ant-on-chain-mcp.antseer.ai/mcp
