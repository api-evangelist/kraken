# Kraken (kraken)

Kraken is one of the world's largest and longest-running cryptocurrency exchanges, founded in 2011 and headquartered in San Francisco. Kraken offers Spot and Futures trading, staking and yield through Kraken Earn, NFT marketplace access, OTC services, custody, prime brokerage, and a B2B Embed surface for partners. Kraken exposes a comprehensive set of APIs spanning REST, WebSocket, and FIX across the Spot exchange, Futures exchange (Kraken Futures, formerly Crypto Facilities), institutional services (Custody, OTC, Prime), and partner integration surfaces (Embed, Ramp, OAuth).

**APIs.json:** [https://docs.kraken.com/api/](https://docs.kraken.com/api/)

## Tags

- Cryptocurrency
- Exchange
- Trading
- Market Data
- Spot Trading
- Futures
- Derivatives
- Staking
- Earn
- NFT
- WebSocket
- FIX
- Custody
- OTC
- Prime Brokerage
- Embed
- OAuth
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Kraken Spot REST API

Public and private REST endpoints for the Kraken Spot exchange. Covers public market data (server time, system status, asset info, ticker, OHLC, order book depth, recent trades, recent spreads), private account data (balances, trade balance, open orders, closed orders, query orders, trades history, query trades, open positions, ledgers, query ledgers, trade volume, API key info), trading (add order, edit order, amend order, cancel order, cancel all, cancel all orders after, add order batch, cancel order batch), funding (deposit methods, deposit addresses, deposit status, withdraw info, withdraw, withdraw status, withdrawal cancel, wallet transfer), subaccounts (create, transfer), Earn (allocate, deallocate, allocations, allocation status, strategies), and the WebSocket token endpoint used to authorize private WebSocket subscriptions.

- **Human URL:** [https://docs.kraken.com/api/docs/rest-api/get-server-time](https://docs.kraken.com/api/docs/rest-api/get-server-time)
- **Base URL:** `https://api.kraken.com`

#### Tags

- Spot
- REST
- Trading
- Market Data
- Funding
- Earn

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/rest-api/get-server-time)
- [API Reference](https://docs.kraken.com/api/docs/category/spot-rest/)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-rest-auth)
- [Rate Limits](https://support.kraken.com/articles/206548367-what-are-the-api-rate-limits)
- [OpenAPI](openapi/kraken-spot-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Spot WebSocket API v2

Real-time market data and private user data over WebSocket v2 using subscribe/unsubscribe semantics. Public channels include ticker (L1), book (L2), trade, ohlc, instrument, and admin frames (status, heartbeat, ping/pong). Authenticated channels include executions and balances. Trading methods include add_order, amend_order, edit_order, cancel_order, cancel_all, cancel_on_disconnect, batch_add, and batch_cancel. The authenticated endpoint requires a token obtained from the Spot REST GetWebSocketsToken operation.

- **Human URL:** [https://docs.kraken.com/api/docs/websocket-v2/ping](https://docs.kraken.com/api/docs/websocket-v2/ping)
- **Base URL:** `wss://ws.kraken.com/v2`

#### Tags

- Spot
- WebSocket
- Market Data
- Trading

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/websocket-v2/)
- [API Reference](https://docs.kraken.com/api/docs/websocket-v2/ping)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-ws-auth)
- [AsyncAPI](asyncapi/kraken-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Spot WebSocket API v1 (Legacy)

Legacy Kraken Spot WebSocket API. Continues to operate alongside v2 but v2 is the recommended path for new integrations. Public channels include ticker, book, trade, ohlc, spread; private channels include ownTrades and openOrders.

- **Human URL:** [https://docs.kraken.com/api/docs/category/websocket-v1](https://docs.kraken.com/api/docs/category/websocket-v1)
- **Base URL:** `wss://ws.kraken.com`

#### Tags

- Spot
- WebSocket
- Legacy

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/websocket-v1)
- [API Reference](https://docs.kraken.com/api/docs/websocket-v1/ping)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Futures REST API

REST API for the Kraken Futures derivatives exchange (formerly Crypto Facilities). Provides trading (send order, edit order, cancel order, cancel all, batch order), market data (instruments, tickers, orderbook, history, recent orders), account data (accounts, open positions, open orders, fills, notifications, account log, transfers, withdrawal), history (account history, execution events, order events, trigger events, market history), charts (candles, analytics), and API key management endpoints.

- **Human URL:** [https://docs.kraken.com/api/docs/futures-api/trading/get-accounts](https://docs.kraken.com/api/docs/futures-api/trading/get-accounts)
- **Base URL:** `https://futures.kraken.com/derivatives/api/v3`

#### Tags

- Futures
- Derivatives
- REST
- Trading

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/futures-api/trading/get-accounts)
- [API Reference](https://docs.kraken.com/api/docs/category/futures-api/)
- [Authentication](https://docs.kraken.com/api/docs/guides/futures-api-auth)
- [OpenAPI](openapi/kraken-futures-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Futures WebSocket API

Real-time market data and private user feeds for Kraken Futures over WebSocket. Public feeds include trade, book, ticker, ticker_lite, heartbeat; private feeds include fills, open_positions, open_orders, account_log, notifications_auth, deposits_withdrawals.

- **Human URL:** [https://docs.kraken.com/api/docs/category/futures-websocket](https://docs.kraken.com/api/docs/category/futures-websocket)
- **Base URL:** `wss://futures.kraken.com/ws/v1`

#### Tags

- Futures
- Derivatives
- WebSocket
- Market Data

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/futures-websocket)
- [API Reference](https://docs.kraken.com/api/docs/futures-websocket/feeds/heartbeat)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken FIX API

FIX 4.4 / 5.0 SP2 protocol access for Kraken Spot and Futures, used by institutional and high-frequency clients. Provides order management (NewOrderSingle, OrderCancelRequest, OrderCancelReplaceRequest, etc.) and market data request flows (MarketDataRequest, MarketDataSnapshot/Refresh).

- **Human URL:** [https://docs.kraken.com/api/docs/category/fix-api/](https://docs.kraken.com/api/docs/category/fix-api/)
- **Base URL:** `colo-london.vip-fix.kraken.com`

#### Tags

- FIX
- Institutional
- Spot
- Futures

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/fix-api/)
- [Authentication](https://docs.kraken.com/api/docs/guides/fix-api-auth)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken NFT API

REST API for Kraken's NFT marketplace surfaces: collections, asset lookups, listings, offers, watchlist, and user portfolio views. The NFT API is consumed alongside the Spot REST API using the same API key authentication scheme.

- **Human URL:** [https://docs.kraken.com/api/docs/category/nft-rest/](https://docs.kraken.com/api/docs/category/nft-rest/)
- **Base URL:** `https://api.kraken.com`

#### Tags

- NFT
- Marketplace
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/nft-rest/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Earn API

REST endpoints for Kraken Earn (staking, yield, rewards). Lists strategies, allocates funds to a strategy, deallocates funds, and surfaces allocation status and reward history.

- **Human URL:** [https://docs.kraken.com/api/docs/rest-api/allocate-strategy](https://docs.kraken.com/api/docs/rest-api/allocate-strategy)
- **Base URL:** `https://api.kraken.com`

#### Tags

- Earn
- Staking
- Yield
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/rest-api/allocate-strategy)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Embed REST API

B2B integration API enabling partners to embed Kraken trading, custody, and Earn capabilities into their own products. Provides user management, assets, deposits, withdrawals, quote-based and custom orders, portfolio, Earn features, and webhooks for real-time event delivery.

- **Human URL:** [https://docs.kraken.com/api/docs/category/embed/](https://docs.kraken.com/api/docs/category/embed/)
- **Base URL:** `https://embed.kraken.com`

#### Tags

- Embed
- B2B
- Partner
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/embed/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken OAuth REST API

OAuth 2.0 authorization surface allowing third-party applications to request scoped delegated access to a Kraken account holder's data and trading capabilities.

- **Human URL:** [https://docs.kraken.com/api/docs/category/oauth/](https://docs.kraken.com/api/docs/category/oauth/)
- **Base URL:** `https://www.kraken.com/oauth`

#### Tags

- OAuth
- Authorization
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/oauth/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Ramp REST API

Fiat on/off-ramp API surface that lets partner applications offer crypto purchase and conversion experiences powered by Kraken liquidity.

- **Human URL:** [https://docs.kraken.com/api/docs/category/ramp/](https://docs.kraken.com/api/docs/category/ramp/)
- **Base URL:** `https://ramp.kraken.com`

#### Tags

- Ramp
- On-Ramp
- Off-Ramp
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/ramp/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Custody REST API

Institutional custody API providing programmatic access to vaulting, sub-vaulting, wallet generation, transfers, and policy/governance configuration for assets held in Kraken Custody.

- **Human URL:** [https://docs.kraken.com/api/docs/category/custody/](https://docs.kraken.com/api/docs/category/custody/)
- **Base URL:** `https://custody.kraken.com`

#### Tags

- Custody
- Institutional
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/custody/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken OTC REST API

Over-the-counter execution API for institutional clients to request quotes (RFQ), execute block trades, and retrieve OTC trade history.

- **Human URL:** [https://docs.kraken.com/api/docs/category/otc/](https://docs.kraken.com/api/docs/category/otc/)
- **Base URL:** `https://otc.kraken.com`

#### Tags

- OTC
- Institutional
- RFQ
- REST

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/otc/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kraken Prime REST + WebSocket + FIX API

Prime brokerage API surface (REST, WebSocket, FIX) for institutional clients consolidating execution, custody, financing, and reporting under a single relationship.

- **Human URL:** [https://docs.kraken.com/api/docs/category/prime/](https://docs.kraken.com/api/docs/category/prime/)
- **Base URL:** `https://prime.kraken.com`

#### Tags

- Prime
- Brokerage
- Institutional
- REST
- WebSocket
- FIX

#### Properties

- [Documentation](https://docs.kraken.com/api/docs/category/prime/)
- [Postman Collection](collections/kraken-futures-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-futures-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/kraken-spot-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kraken-spot-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://www.kraken.com/)
- [Portal](https://docs.kraken.com/api/)
- [Getting Started](https://docs.kraken.com/api/docs/guides/global-intro)
- [Sign Up](https://www.kraken.com/sign-up)
- [Authentication](https://docs.kraken.com/api/docs/guides/spot-rest-auth)
- [Pricing](https://www.kraken.com/features/fee-schedule)
- [Terms of Service](https://www.kraken.com/legal)
- [Privacy Policy](https://www.kraken.com/legal/privacy)
- [Blog](https://blog.kraken.com/)
- [Status Page](https://status.kraken.com/)
- [Support](https://support.kraken.com/)
- [F A Q](https://support.kraken.com/categories/360001393671-Trading-Funding)
- [GitHub Organization](https://github.com/krakenfx)
- [GitHub Organization](https://github.com/CryptoFacilities)
- [SDK](https://github.com/krakenfx/api-go)
- [SDK](https://github.com/krakenfx/kraken-api-client)
- [SDK](https://github.com/krakenfx/kraken-wsclient-py)
- [SDK](https://github.com/CryptoFacilities/REST-v3-Python)
- [SDK](https://github.com/CryptoFacilities/REST-v3-Java)
- [SDK](https://github.com/CryptoFacilities/REST-v3-CSharp)
- [SDK](https://github.com/CryptoFacilities/REST-v3-NodeJs)
- [SDK](https://github.com/CryptoFacilities/REST-v3-kotlin)
- [SDK](https://github.com/CryptoFacilities/WebSocket-v1-Python)
- [SDK](https://github.com/CryptoFacilities/WebSocket-v1-CSharp)
- [SDK](https://github.com/CryptoFacilities/WebSocket-v1-Rust)
- [C L I](https://github.com/krakenfx/kraken-cli)
- [Tools](https://github.com/krakenfx/kraken-cli)
- [Tools](https://github.com/oilst/kraken-mcp)
- [Tools](https://github.com/krakenfx/wallet)
- [Spectral Rules](rules/kraken-rules.yml)
- [Vocabulary](vocabulary/kraken-vocabulary.yml)
- [J S O N- L D](json-ld/kraken-context.jsonld)
- [Plans](plans/kraken-plans-pricing.yml)
- [Rate Limits](rate-limits/kraken-rate-limits.yml)
- [Fin Ops](finops/kraken-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
