# Kraken (kraken)

Kraken is one of the world's largest and longest-running cryptocurrency exchanges, founded in 2011 and headquartered in San Francisco. Kraken offers Spot and Futures trading, staking and yield through Kraken Earn, NFT marketplace access, OTC services, custody, prime brokerage, and a B2B Embed surface for partners. Kraken exposes a comprehensive set of APIs spanning REST, WebSocket, and FIX across the Spot exchange, Futures exchange (Kraken Futures, formerly Crypto Facilities), institutional services (Custody, OTC, Prime), and partner integration surfaces (Embed, Ramp, OAuth).

**URL:** [Visit APIs.json URL](https://docs.kraken.com/api/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Cryptocurrency, Exchange, Trading, Market Data, Spot Trading, Futures, Derivatives, Staking, Earn, NFT, WebSocket, FIX, Custody, OTC, Prime Brokerage, Embed, OAuth, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Kraken Spot REST API

Public and private REST endpoints for the Kraken Spot exchange. Covers public market data, account data, trading, funding, subaccounts, Earn, and the WebSocket token endpoint.

**Human URL:** [https://docs.kraken.com/api/docs/rest-api/get-server-time](https://docs.kraken.com/api/docs/rest-api/get-server-time)

#### Tags

- Spot, REST, Trading, Market Data, Funding, Earn

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/rest-api/get-server-time)
- [APIReference](https://docs.kraken.com/api/docs/category/spot-rest/)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-rest-auth)
- [RateLimits](https://support.kraken.com/articles/206548367-what-are-the-api-rate-limits)
- [OpenAPI](openapi/kraken-spot-rest-openapi.yml)
- [NaftikoCapability — Market Data](capabilities/spot-rest-market-data.yaml)
- [NaftikoCapability — Account Data](capabilities/spot-rest-account-data.yaml)
- [NaftikoCapability — Trading](capabilities/spot-rest-trading.yaml)
- [NaftikoCapability — Funding](capabilities/spot-rest-funding.yaml)
- [NaftikoCapability — Subaccounts](capabilities/spot-rest-subaccounts.yaml)
- [NaftikoCapability — Earn](capabilities/spot-rest-earn.yaml)
- [NaftikoCapability — WebSocket Token](capabilities/spot-rest-websocket.yaml)

### Kraken Spot WebSocket API v2

Real-time market data and private user data over WebSocket v2 using subscribe/unsubscribe semantics.

**Human URL:** [https://docs.kraken.com/api/docs/websocket-v2/ping](https://docs.kraken.com/api/docs/websocket-v2/ping)

#### Tags

- Spot, WebSocket, Market Data, Trading

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/websocket-v2/)
- [APIReference](https://docs.kraken.com/api/docs/websocket-v2/ping)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-ws-auth)
- [AsyncAPI](asyncapi/kraken-asyncapi.yml)
- [NaftikoCapability — Streams](capabilities/spot-websocket-v2-streams.yaml)

### Kraken Spot WebSocket API v1 (Legacy)

Legacy Kraken Spot WebSocket API. Continues to operate alongside v2 but v2 is the recommended path for new integrations.

**Human URL:** [https://docs.kraken.com/api/docs/category/websocket-v1](https://docs.kraken.com/api/docs/category/websocket-v1)

### Kraken Futures REST API

REST API for the Kraken Futures derivatives exchange (formerly Crypto Facilities). Trading, market data, account data, history, charts, and API key management.

**Human URL:** [https://docs.kraken.com/api/docs/futures-api/trading/get-accounts](https://docs.kraken.com/api/docs/futures-api/trading/get-accounts)

#### Tags

- Futures, Derivatives, REST, Trading

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/futures-api/trading/get-accounts)
- [APIReference](https://docs.kraken.com/api/docs/category/futures-api/)
- [Authentication](https://docs.kraken.com/api/docs/guides/futures-api-auth)
- [OpenAPI](openapi/kraken-futures-rest-openapi.yml)
- [NaftikoCapability — Market Data](capabilities/futures-rest-market-data.yaml)
- [NaftikoCapability — Account](capabilities/futures-rest-account.yaml)
- [NaftikoCapability — Trading](capabilities/futures-rest-trading.yaml)
- [NaftikoCapability — Transfers](capabilities/futures-rest-transfers.yaml)
- [NaftikoCapability — History](capabilities/futures-rest-history.yaml)
- [NaftikoCapability — Charts](capabilities/futures-rest-charts.yaml)
- [NaftikoCapability — Auth](capabilities/futures-rest-auth.yaml)

### Kraken Futures WebSocket API

Real-time market data and private user feeds for Kraken Futures over WebSocket.

**Human URL:** [https://docs.kraken.com/api/docs/category/futures-websocket](https://docs.kraken.com/api/docs/category/futures-websocket)

### Kraken FIX API

FIX 4.4 / 5.0 SP2 protocol access for Kraken Spot and Futures, used by institutional and high-frequency clients.

**Human URL:** [https://docs.kraken.com/api/docs/category/fix-api/](https://docs.kraken.com/api/docs/category/fix-api/)

### Kraken NFT API

REST API for Kraken's NFT marketplace surfaces: collections, asset lookups, listings, offers, watchlist, and user portfolio.

**Human URL:** [https://docs.kraken.com/api/docs/category/nft-rest/](https://docs.kraken.com/api/docs/category/nft-rest/)

### Kraken Earn API

REST endpoints for Kraken Earn (staking, yield, rewards).

**Human URL:** [https://docs.kraken.com/api/docs/rest-api/allocate-strategy](https://docs.kraken.com/api/docs/rest-api/allocate-strategy)

### Kraken Embed REST API

B2B integration API enabling partners to embed Kraken trading, custody, and Earn capabilities into their own products.

**Human URL:** [https://docs.kraken.com/api/docs/category/embed/](https://docs.kraken.com/api/docs/category/embed/)

### Kraken OAuth REST API

OAuth 2.0 authorization surface allowing third-party applications to request scoped delegated access.

**Human URL:** [https://docs.kraken.com/api/docs/category/oauth/](https://docs.kraken.com/api/docs/category/oauth/)

### Kraken Ramp REST API

Fiat on/off-ramp API surface that lets partner applications offer crypto purchase and conversion experiences powered by Kraken liquidity.

**Human URL:** [https://docs.kraken.com/api/docs/category/ramp/](https://docs.kraken.com/api/docs/category/ramp/)

### Kraken Custody REST API

Institutional custody API providing programmatic access to vaulting, sub-vaulting, wallet generation, transfers, and policy/governance.

**Human URL:** [https://docs.kraken.com/api/docs/category/custody/](https://docs.kraken.com/api/docs/category/custody/)

### Kraken OTC REST API

Over-the-counter execution API for institutional clients to request quotes (RFQ), execute block trades, and retrieve OTC trade history.

**Human URL:** [https://docs.kraken.com/api/docs/category/otc/](https://docs.kraken.com/api/docs/category/otc/)

### Kraken Prime REST + WebSocket + FIX API

Prime brokerage API surface consolidating execution, custody, financing, and reporting under a single relationship.

**Human URL:** [https://docs.kraken.com/api/docs/category/prime/](https://docs.kraken.com/api/docs/category/prime/)

## Common Properties

- [Website](https://www.kraken.com/)
- [Portal](https://docs.kraken.com/api/)
- [GettingStarted](https://docs.kraken.com/api/docs/guides/global-intro)
- [SignUp](https://www.kraken.com/sign-up)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-rest-auth)
- [Pricing](https://www.kraken.com/features/fee-schedule)
- [TermsOfService](https://www.kraken.com/legal)
- [PrivacyPolicy](https://www.kraken.com/legal/privacy)
- [Blog](https://blog.kraken.com/)
- [StatusPage](https://status.kraken.com/)
- [Support](https://support.kraken.com/)
- [FAQ](https://support.kraken.com/categories/360001393671-Trading-Funding)
- [GitHubOrganization — krakenfx](https://github.com/krakenfx)
- [GitHubOrganization — CryptoFacilities](https://github.com/CryptoFacilities)
- [SDK — Kraken Go SDK](https://github.com/krakenfx/api-go)
- [SDK — Kraken PHP API Client](https://github.com/krakenfx/kraken-api-client)
- [SDK — Kraken Python WebSocket Client](https://github.com/krakenfx/kraken-wsclient-py)
- [SDK — Crypto Facilities REST v3 Python](https://github.com/CryptoFacilities/REST-v3-Python)
- [SDK — Crypto Facilities REST v3 Java](https://github.com/CryptoFacilities/REST-v3-Java)
- [SDK — Crypto Facilities REST v3 C#](https://github.com/CryptoFacilities/REST-v3-CSharp)
- [SDK — Crypto Facilities REST v3 Node.js](https://github.com/CryptoFacilities/REST-v3-NodeJs)
- [SDK — Crypto Facilities REST v3 Kotlin](https://github.com/CryptoFacilities/REST-v3-kotlin)
- [SDK — Crypto Facilities WebSocket v1 Python](https://github.com/CryptoFacilities/WebSocket-v1-Python)
- [SDK — Crypto Facilities WebSocket v1 C#](https://github.com/CryptoFacilities/WebSocket-v1-CSharp)
- [SDK — Crypto Facilities WebSocket v1 Rust](https://github.com/CryptoFacilities/WebSocket-v1-Rust)
- [CLI — Kraken CLI (Rust, AI-native, MCP-capable)](https://github.com/krakenfx/kraken-cli)
- [Tools — Kraken CLI MCP Server (official)](https://github.com/krakenfx/kraken-cli)
- [Tools — oilst/kraken-mcp (community FastMCP server)](https://github.com/oilst/kraken-mcp)
- [Tools — Kraken Wallet (self-custody)](https://github.com/krakenfx/wallet)
- [SpectralRules](rules/kraken-rules.yml)
- [Vocabulary](vocabulary/kraken-vocabulary.yml)
- [JSON-LD](json-ld/kraken-context.jsonld)
- [Plans](plans/kraken-plans-pricing.yml)
- [RateLimits](rate-limits/kraken-rate-limits.yml)
- [FinOps](finops/kraken-finops.yml)

## Features

| Name | Description |
|------|-------------|
| Spot Trading | 200+ pairs with limit/market/stop/take-profit/trailing-stop/iceberg/settle-position order types |
| Margin Trading | Up to 5x leverage on eligible pairs and jurisdictions |
| Futures Trading | Perpetual and fixed-maturity futures on BTC, ETH, and other majors |
| Kraken Earn | On-chain and off-chain staking plus bonded yield strategies |
| NFT Marketplace | ETH + Solana NFTs with gas-free transactions and fiat settlement |
| Subaccounts | Logical subaccount creation and inter-account transfers |
| Embed (B2B Integration) | White-label trading, custody, and Earn primitives |
| OAuth Delegated Access | Scoped third-party app access via OAuth 2.0 |
| Co-located Connectivity | London colocation endpoints for low-latency access |
| FIX Connectivity | FIX 4.4 / 5.0 SP2 for institutional execution |
| WebSocket v2 with Authenticated Trading | Modern WS surface for market data and trading methods |
| Cancel on Disconnect | Auto-cancel resting orders on session termination |

## Use Cases

| Name | Description |
|------|-------------|
| Algorithmic Spot Trading | REST for order management + WebSocket v2 for low-latency feeds |
| Cross-Exchange Arbitrage | Real-time books + colocation endpoints |
| Derivatives Market Making | Batched orders + WS fills + FIX |
| Treasury and Custody Operations | Programmatic transfers + custody |
| Staking-as-a-Service | Programmatic Earn allocation/deallocation |
| Embedded Crypto Brokerage | Kraken Embed for partner apps |
| NFT Portfolio Management | Portfolio dashboards + collection analytics |
| AI Agent Trading | Kraken CLI MCP server + community Kraken MCP for LLM agents |
| Tax and Reporting Pipelines | Trades, ledgers, deposits, withdrawals for tax/audit |

## Integrations

| Name | Description |
|------|-------------|
| Crypto Facilities (Kraken Futures) | Public REST v3 + WS v1 example clients in multiple languages |
| Kraken Wallet | Self-custody wallet integrating with dApps + Kraken OAuth |
| Model Context Protocol | Kraken CLI embeds MCP server for Claude/Gemini/Cursor |
| TradingView | Kraken markets as TradingView charting source; embedded in Kraken Pro |
| CCXT | First-class exchange adapter in CCXT |

## Solutions

| Name | Description |
|------|-------------|
| Kraken | Simplified consumer app — 1.0% / 1.5% spread |
| Kraken Pro | Advanced trading — 0.25%/0.40% down to 0.00%/0.10% at $10M+ |
| Kraken Institutional | Custody + OTC + Prime + colocation + FIX |
| Kraken Embed | B2B partner platform for trading/custody/Earn |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Kraken Spot REST API](openapi/kraken-spot-rest-openapi.yml) — 46 paths, 86 schemas, Microcks-compatible inline examples
- [Kraken Futures REST API](openapi/kraken-futures-rest-openapi.yml) — 25 paths, 9 schemas, Microcks-compatible inline examples

### AsyncAPI

- [Kraken Spot WebSocket API v2](asyncapi/kraken-asyncapi.yml) — 6 channels (ticker, book, ohlc, trade, instrument, system), 18 messages

### JSON Schema

117 standalone JSON Schema (draft 2020-12) files extracted from the OpenAPI specs, one per component schema. See [`json-schema/`](json-schema/).

### JSON Structure

117 JSON Structure (v0) projections matching the JSON Schema set. See [`json-structure/`](json-structure/).

### JSON-LD

- [Kraken JSON-LD Context](json-ld/kraken-context.jsonld) — maps Kraken core entities (Asset, AssetPair, Ticker, OrderBook, Order, Trade, Position, Balance, LedgerEntry, Instrument, EarnStrategy, EarnAllocation, FundingTxn) to schema.org and FIBO equivalents

### Examples

71 ready-to-replay JSON examples for every 2xx response in the OpenAPI specs. See [`examples/`](examples/).

## Capabilities

Naftiko capabilities organized as one self-contained file per business surface (OpenAPI tag). Each file inlines its own `consumes` + REST + MCP exposers.

| Capability | API | Operations | File |
|-----------|-----|------------|------|
| Spot REST — Market Data | Spot REST | 9 | [spot-rest-market-data.yaml](capabilities/spot-rest-market-data.yaml) |
| Spot REST — Account Data | Spot REST | 12 | [spot-rest-account-data.yaml](capabilities/spot-rest-account-data.yaml) |
| Spot REST — Trading | Spot REST | 8 | [spot-rest-trading.yaml](capabilities/spot-rest-trading.yaml) |
| Spot REST — Funding | Spot REST | 8 | [spot-rest-funding.yaml](capabilities/spot-rest-funding.yaml) |
| Spot REST — Subaccounts | Spot REST | 2 | [spot-rest-subaccounts.yaml](capabilities/spot-rest-subaccounts.yaml) |
| Spot REST — Earn | Spot REST | 6 | [spot-rest-earn.yaml](capabilities/spot-rest-earn.yaml) |
| Spot REST — WebSocket Token | Spot REST | 1 | [spot-rest-websocket.yaml](capabilities/spot-rest-websocket.yaml) |
| Spot WebSocket v2 — Streams | Spot WS v2 | 12 | [spot-websocket-v2-streams.yaml](capabilities/spot-websocket-v2-streams.yaml) |
| Futures REST — Market Data | Futures REST | 6 | [futures-rest-market-data.yaml](capabilities/futures-rest-market-data.yaml) |
| Futures REST — Account | Futures REST | 5 | [futures-rest-account.yaml](capabilities/futures-rest-account.yaml) |
| Futures REST — Trading | Futures REST | 6 | [futures-rest-trading.yaml](capabilities/futures-rest-trading.yaml) |
| Futures REST — Transfers | Futures REST | 2 | [futures-rest-transfers.yaml](capabilities/futures-rest-transfers.yaml) |
| Futures REST — History | Futures REST | 4 | [futures-rest-history.yaml](capabilities/futures-rest-history.yaml) |
| Futures REST — Charts | Futures REST | 1 | [futures-rest-charts.yaml](capabilities/futures-rest-charts.yaml) |
| Futures REST — Auth | Futures REST | 1 | [futures-rest-auth.yaml](capabilities/futures-rest-auth.yaml) |

## Vocabulary

- [Kraken Vocabulary](vocabulary/kraken-vocabulary.yml) — 32 domain concepts mapping Spot, Futures, NFT, Earn, FIX, OAuth, and MCP primitives to schema.org / FIBO references where applicable

## Rules

- [Kraken Spectral Ruleset](rules/kraken-rules.yml) — 36 rules across 12 categories enforcing Kraken's documented naming, security, response envelope, and HTTP method conventions

## Plans, Rate Limits, and FinOps

- [Kraken Plans + Pricing](plans/kraken-plans-pricing.yml) — 8 plans covering consumer (Kraken + Kraken+), Pro Spot (volume-tiered standard + stablecoin), Futures, Earn, Institutional, and Embed
- [Kraken Rate Limits](rate-limits/kraken-rate-limits.yml) — Per-tier API counter (Starter/Intermediate/Pro), WebSocket connection caps, FIX session negotiation, and 8 documented policies
- [Kraken FinOps](finops/kraken-finops.yml) — FOCUS 1.3 aligned, 9 meters covering spot/futures take rate, consumer app, Kraken+, funding, Earn (allocation + reward), and NFT marketplace fees

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
