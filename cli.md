# Antseer CLI

[中文](#中文) · [日本語](#日本語) · [한국어](#한국어)

A standalone command-line tool for querying Web3 data directly from your terminal, powered by the Antseer data platform.

---

## Installation

### macOS / Linux

```bash
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash
```

### Windows (PowerShell)

```powershell
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

After installation, restart your terminal and run:

```bash
antseer --help
```

---

## Configuration

Connect to the Antseer service:

```bash
antseer auth --server-url https://ant-on-chain-mcp.antseer.ai
```

---

## Usage

```bash
# Show available commands
antseer --help

# Show version
antseer --version

# List all available data tools
antseer tools

# Query data (table output by default)
antseer <tool> <query-type> --params '<json>'

# Machine-readable JSON output (for agent consumption)
antseer <tool> <query-type> --params '<json>' -o json
```

### Examples

```bash
# Top DeFi protocols by TVL
antseer protocol tvl --params '{"limit": 10}'

# BTC funding rates across exchanges
antseer futures funding-rate --params '{"symbol": "BTC"}'

# Bitcoin ETF fund flows
antseer etf btc-etf-list

# Stablecoin market overview
antseer stablecoin overview

# Macro: US GDP data
antseer macro real-gdp --params '{"interval": "annual"}'

# Market sentiment
antseer sentiment coin-of-the-day
```

---

## Output Formats

| Flag | Description |
|------|-------------|
| *(default)* | Human-readable table |
| `-o json` / `--json` | JSON output for agent/script consumption |

---

## Interactive REPL

Run without arguments to enter interactive mode:

```bash
antseer
```

Type `help` for available commands, `quit` to exit.

---

## Links

- **Website:** https://antseer.ai
- **MCP Endpoint:** https://ant-on-chain-mcp.antseer.ai/mcp

---

## 中文

**安装**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows（PowerShell）
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

**配置**

```bash
antseer auth --server-url https://ant-on-chain-mcp.antseer.ai
```

**常用命令**

```bash
antseer tools                                          # 列出所有工具
antseer protocol tvl --params '{"limit": 10}'         # DeFi 协议 TVL
antseer futures funding-rate --params '{"symbol": "BTC"}'  # BTC 资金费率
antseer etf btc-etf-list                               # 比特币 ETF 资金流
antseer macro real-gdp --params '{"interval": "annual"}'   # 美国 GDP
```

---

## 日本語

**インストール**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows（PowerShell）
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

**設定**

```bash
antseer auth --server-url https://ant-on-chain-mcp.antseer.ai
```

**主なコマンド**

```bash
antseer tools                                          # 利用可能なツール一覧
antseer protocol tvl --params '{"limit": 10}'         # DeFiプロトコルTVL
antseer futures funding-rate --params '{"symbol": "BTC"}'  # BTC資金調達率
antseer etf btc-etf-list                               # ビットコインETF資金フロー
antseer macro real-gdp --params '{"interval": "annual"}'   # 米国GDP
```

---

## 한국어

**설치**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows (PowerShell)
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

**설정**

```bash
antseer auth --server-url https://ant-on-chain-mcp.antseer.ai
```

**주요 명령어**

```bash
antseer tools                                          # 사용 가능한 툴 목록
antseer protocol tvl --params '{"limit": 10}'         # DeFi 프로토콜 TVL
antseer futures funding-rate --params '{"symbol": "BTC"}'  # BTC 펀딩 비율
antseer etf btc-etf-list                               # 비트코인 ETF 자금 흐름
antseer macro real-gdp --params '{"interval": "annual"}'   # 미국 GDP
```
