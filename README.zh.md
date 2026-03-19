# Antseer — Agent 时代的 Web3 数据操作系统

**[官网](https://antseer.ai)** · [English](README.md) · [日本語](README.ja.md) · [한국어](README.ko.md)

![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-green) ![Tools](https://img.shields.io/badge/tools-100%2B-blue) ![No API Key](https://img.shields.io/badge/API%20Key-Not%20Required-brightgreen) ![CLI](https://img.shields.io/badge/CLI-v1.3.0-orange)

> 单一 MCP 端点，100+ 实时 Web3 数据工具，无需 API Key。

Antseer 通过单一 [Model Context Protocol (MCP)](https://modelcontextprotocol.io) 端点，将 AI Agent 与实时链上数据和市场情报直接连接。任何兼容 MCP 的客户端连接后即可自动发现所有可用工具，无需 SDK，无需配置，无需 API Key。

---

## 快速接入

**MCP 端点：** `https://ant-on-chain-mcp.antseer.ai/mcp`

### Claude Code

```bash
claude mcp add antseer --transport http https://ant-on-chain-mcp.antseer.ai/mcp
```

### Claude Desktop

在 `claude_desktop_config.json` 中添加：

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

在 MCP 设置中添加：

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

## 数据分类

100+ 工具，覆盖四大数据域，由多家专业 Web3 数据提供商驱动。

### 🔗 链上（OnChain）
- 协议 TVL、收益率、手续费与收入追踪
- 聪明钱与巨鲸钱包监控
- 跨链桥资金流向
- 稳定币市场动态与供应分析
- Meme 币叙事检测与分析
- 代币链上指标、持仓分布与盈亏分析
- 钱包地址画像与交易对手分析

### 📊 中心化金融（CeFi）
- 现货市场结构、价格与订单簿深度
- 期货未平仓量、资金费率与清算追踪
- 市场技术指标
- 永续 DEX 分析与巨鲸持仓追踪

### 🏦 传统金融（TradFi）
- 比特币与以太坊 ETF 净流入与 AUM
- 代币化美股（价格、历史、K 线）
- 代币化贵金属

### 🌍 宏观与情绪（Macro & Sentiment）
- 美国宏观经济指标 — GDP、CPI、联邦基金利率、国债收益率、失业率
- 加密市场情绪评分与社交数据分析

---

## 查询示例

接入后，直接用自然语言向 AI Agent 提问：

- *"按 TVL 列出前 10 大 DeFi 协议及其 7 日变化"*
- *"当前各大交易所的 BTC 资金费率是多少？"*
- *"本周比特币 ETF 净流入了多少？"*
- *"过去 24 小时哪些钱包在持续买入 ETH？"*
- *"当前市场恐慌贪婪指数和情绪如何？"*

---

## CLI 工具

Antseer 同时提供独立 CLI 工具，支持在终端直接查询数据。

→ 详见 [cli.md](cli.md)

**快速安装：**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows（PowerShell）
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

---

## 联系我们

- 邮箱：[antseersupport@antseer.ai](mailto:antseersupport@antseer.ai)
- Twitter / X：[@Antseer_ai](https://x.com/Antseer_ai)
- Telegram：[t.me/antseer](https://t.me/antseer)
- 官网：[antseer.ai](https://antseer.ai)
