# Kraken GraphQL Schema

This document describes a conceptual GraphQL schema for the Kraken cryptocurrency exchange API. Kraken's public API is REST and WebSocket based (see the [Kraken REST API docs](https://docs.kraken.com/api/docs/rest-api/get-server-time) and [WebSocket v2 docs](https://docs.kraken.com/api/docs/websocket-v2/ping)), but the types here model the full breadth of Kraken's domain objects across Spot trading, Futures, Earn, NFT, funding, and account management surfaces.

## Schema Source

- **Provider:** Kraken (https://www.kraken.com/)
- **API Documentation:** https://docs.kraken.com/api/
- **GitHub (community client):** https://github.com/nickcoutsos/kraken-api
- **Schema file:** `kraken-schema.graphql`
- **Type count:** 57 named types

## Coverage

The schema covers the following Kraken API surfaces:

### Public Market Data
- `SystemStatus`, `ServerTime` — system health and time endpoints
- `AssetInfo`, `AssetPair` — tradeable assets and trading pairs metadata
- `Ticker`, `OHLCV`, `Depth`, `OrderBookEntry`, `Trade`, `Spread` — live and historical market data

### Private Account Data
- `AccountBalance`, `TradeBalance`, `MarginCallLevel`, `MarginFreeLevel` — balance and margin information
- `OpenOrder`, `ClosedOrder`, `TradesHistory`, `OpenPosition` — order and trade history
- `Ledger`, `TradeVolume`, `FeeInfo`, `VolumeDiscount` — ledger entries and fee/volume data
- `APIKeyInfo`, `TWOFAType`, `TokenInfo` — API key and authentication metadata

### Trading
- `AddOrder`, `CancelOrder`, `OrderDescription`, `OrderFlags`, `UserRef`, `TransactionId` — order lifecycle
- `Margin` — margin position data

### Funding
- `DepositMethod`, `DepositAddress`, `DepositStatus` — deposit flows
- `WithdrawInfo`, `WithdrawStatus`, `WithdrawalCancel` — withdrawal flows

### Earn / Staking
- `Staking`, `StakingAsset`, `PendingStaking`, `TransactionType` — Earn and staking management

### Export / Reporting
- `ExportReport`, `ExportStatus` — trade and ledger data exports

### NFT
- `NFTInfo`, `NFTBid`, `NFTAuction`, `NFTCollection` — NFT marketplace objects

## Query and Mutation Roots

The schema exposes:

- **Query** — read operations for market data and account state
- **Mutation** — write operations for placing/canceling orders, funding, Earn allocation

## Notes

This schema is conceptual and maps Kraken's REST domain model into GraphQL types. It is intended for tooling, documentation, and schema-driven development workflows. Kraken does not currently offer a native GraphQL endpoint.
