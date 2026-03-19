# Antseer — エージェント時代のWeb3データOS

**[公式サイト](https://antseer.ai)** · [English](README.md) · [中文](README.zh.md) · [한국어](README.ko.md)

> 単一のMCPエンドポイント。100以上のリアルタイムWeb3データツール。APIキー不要。

Antseerは、単一の[Model Context Protocol (MCP)](https://modelcontextprotocol.io)エンドポイントを通じて、AIエージェントをリアルタイムのオンチェーンデータとマーケットインテリジェンスに接続します。MCP対応クライアントは接続時にすべての利用可能なツールを自動検出します。SDK不要、設定不要、APIキー不要。

---

## クイック接続

**MCPエンドポイント：** `https://ant-on-chain-mcp.antseer.ai/mcp`

### Claude Code

```bash
claude mcp add antseer --transport http https://ant-on-chain-mcp.antseer.ai/mcp
```

### Claude Desktop

`claude_desktop_config.json` に追加：

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

MCP設定に追加：

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

## データカテゴリ

複数のプロフェッショナルなWeb3データプロバイダーによる、4つのドメインにわたる100以上のツール。

### オンチェーン（OnChain）
- プロトコルTVL、利回り、手数料・収益トラッキング
- スマートマネー・クジラウォレット監視
- クロスチェーンブリッジ資金フロー
- ステーブルコイン市場動向・供給分析
- ミームトークンのナラティブ検出・分析
- トークンオンチェーン指標、保有分布・損益分析
- ウォレットアドレスプロファイリング・取引相手分析

### 中央集権型金融（CeFi）
- 現物市場構造、価格・オーダーブック深度
- 先物建玉、資金調達率・清算トラッキング
- 市場テクニカル指標
- 永続DEX分析・クジラポジション追跡

### 伝統的金融（TradFi）
- ビットコイン・イーサリアムETFの純流入・AUM
- トークン化米国株（価格、履歴、OHLC）
- トークン化貴金属

### マクロ・センチメント（Macro & Sentiment）
- 米国マクロ経済指標 — GDP、CPI、FF金利、国債利回り、失業率
- 暗号資産市場センチメントスコア・ソーシャルデータ分析

---

## クエリ例

接続後、AIエージェントに自然言語で質問できます：

- *「TVL上位10のDeFiプロトコルと7日間の変化を教えて」*
- *「主要取引所のBTC資金調達率は今いくら？」*
- *「今週のビットコインETF純流入額は？」*
- *「過去24時間でETHを買い増しているウォレットは？」*
- *「現在の恐怖・貪欲指数と市場センチメントは？」*

---

## CLIツール

AntseerはターミナルからデータをクエリできるスタンドアロンCLIも提供しています。

→ インストールと使い方は [cli.md](cli.md) を参照

**クイックインストール：**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows（PowerShell）
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

---

## リンク

- **公式サイト：** https://antseer.ai
- **MCPエンドポイント：** https://ant-on-chain-mcp.antseer.ai/mcp
