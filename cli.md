# Antseer CLI

> A standalone command-line tool for querying Web3 data directly from your terminal.

![version](https://img.shields.io/badge/version-1.3.0-blue) ![platform](https://img.shields.io/badge/platform-macOS%20%7C%20Linux%20%7C%20Windows-lightgrey)

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

## Contact

- Email: [antseersupport@antseer.ai](mailto:antseersupport@antseer.ai)
- Twitter / X: [@Antseer_ai](https://x.com/Antseer_ai)
- Telegram: [t.me/antseer](https://t.me/antseer)
- Website: [antseer.ai](https://antseer.ai)
