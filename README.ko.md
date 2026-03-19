# Antseer — 에이전트 시대의 Web3 데이터 OS

**[공식 웹사이트](https://antseer.ai)** · [English](README.md) · [中文](README.zh.md) · [日本語](README.ja.md)

> 단일 MCP 엔드포인트. 100개 이상의 실시간 Web3 데이터 툴. API 키 불필요.

Antseer는 단일 [Model Context Protocol (MCP)](https://modelcontextprotocol.io) 엔드포인트를 통해 AI 에이전트를 실시간 온체인 데이터 및 시장 인텔리전스에 연결합니다. MCP 호환 클라이언트는 연결 시 모든 사용 가능한 툴을 자동으로 검색합니다. SDK 불필요, 설정 불필요, API 키 불필요.

---

## 빠른 연결

**MCP 엔드포인트:** `https://ant-on-chain-mcp.antseer.ai/mcp`

### Claude Code

```bash
claude mcp add antseer --transport http https://ant-on-chain-mcp.antseer.ai/mcp
```

### Claude Desktop

`claude_desktop_config.json`에 추가:

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

MCP 설정에 추가:

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

## 데이터 카테고리

여러 전문 Web3 데이터 제공업체가 지원하는 4개 도메인의 100개 이상 툴.

### 온체인 (OnChain)
- 프로토콜 TVL, 수익률, 수수료 및 수익 추적
- 스마트 머니 및 고래 지갑 모니터링
- 크로스체인 브릿지 자금 흐름
- 스테이블코인 시장 동향 및 공급 분석
- 밈 토큰 내러티브 감지 및 분석
- 토큰 온체인 지표, 보유 분포 및 손익 분석
- 지갑 주소 프로파일링 및 거래 상대방 분석

### 중앙화 금융 (CeFi)
- 현물 시장 구조, 가격 및 오더북 깊이
- 선물 미결제약정, 펀딩 비율 및 청산 추적
- 시장 기술 지표
- 무기한 DEX 분석 및 고래 포지션 추적

### 전통 금융 (TradFi)
- 비트코인 및 이더리움 ETF 순유입 및 AUM
- 토큰화 미국 주식 (가격, 이력, OHLC)
- 토큰화 귀금속

### 거시경제 및 심리 (Macro & Sentiment)
- 미국 거시경제 지표 — GDP, CPI, 연방기금금리, 국채 수익률, 실업률
- 암호화폐 시장 심리 점수 및 소셜 데이터 분석

---

## 쿼리 예시

연결 후 AI 에이전트에게 자연어로 질문하세요:

- *"TVL 기준 상위 10개 DeFi 프로토콜과 7일 변화를 보여줘"*
- *"지금 주요 거래소의 BTC 펀딩 비율은?"*
- *"이번 주 비트코인 ETF 순유입액은 얼마야?"*
- *"지난 24시간 동안 ETH를 매집하는 지갑은 어디야?"*
- *"현재 공포 탐욕 지수와 시장 심리는?"*

---

## CLI 툴

Antseer는 터미널에서 직접 데이터를 쿼리할 수 있는 독립형 CLI도 제공합니다.

→ 설치 및 사용법은 [cli.md](cli.md) 참조

**빠른 설치:**

```bash
# macOS / Linux
curl -sSfL https://skillhub-api.antseer.ai/files/clis/install.sh | bash

# Windows (PowerShell)
irm https://skillhub-api.antseer.ai/files/clis/install.ps1 | iex
```

---

## 링크

- **공식 웹사이트:** https://antseer.ai
- **MCP 엔드포인트:** https://ant-on-chain-mcp.antseer.ai/mcp
