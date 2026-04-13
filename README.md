# Yahya Ehsan

**Trading Systems Engineer**

High performance infrastructure for prediction markets and algorithmic trading.
Rust for microsecond latency execution systems, with a research layer for
identifying and systematizing exploitable market inefficiencies.

**Currently:** Quant researcher + systems engineer on Polymarket —
building and validating alpha-generating strategies backed by data,
with production Rust execution infrastructure.

**Focus areas:** Market microstructure analysis, pricing inefficiency detection,
order book dynamics, automated execution with risk controls.

---

## Trading & Research Work

### Polymarket Alpha Research Infrastructure

End-to-end pipeline for prediction market strategy development:
research → backtest → production execution.

**Research layer:**
- Arbitrage detection across correlated Polymarket markets (CLOB API)
- Order book microstructure analysis: spread patterns, liquidity depth, price impact
- Pricing inefficiency identification via real-time WebSocket order book streaming
- Signal generation from cross-market dislocations and event-driven mispricings

**Execution layer:**
- 4 independent async executors with isolated failure domains
- Sub-100ms market state detection, <1ms message processing
- Event-driven architecture: raw market data → normalized signals → execution
- Kill switch, position sizing logic, automated risk controls
- Zero shared mutable state across await points

**Stack:** Rust, Tokio, WebSockets, Polymarket CLOB API  
**Latency:** Round detection <100ms · Message processing <1ms · 10-20MB RSS per asset

---

## Other Systems Projects

### Real-Time File Sync Engine
High-performance file sync with AES-256-GCM encryption and async I/O.  
**Performance:** 123µs avg sync time across 5000+ files · **Stack:** Rust, Tokio

### Redis Clone
Thread-safe in-memory KV store with custom benchmarking framework.  
**Performance:** SET 381ns/op · GET 16.8ns/op (M1) · **Stack:** Go

### Google Calendar OAuth & Incremental Sync
OAuth 2.0 with incremental sync via `nextSyncToken`. 10-100x faster than full sync.  
**Performance:** Full sync ~2-5s · Incremental ~200-500ms · **Stack:** TypeScript, Node.js

### RISC-V OS Kernel
Bare-metal kernel: SV32 virtual memory, process management, context switching.  
**Stack:** Rust, RISC-V assembly

---

## Technical Stack

**Core:** Rust (Tokio, async/await, lock-free concurrency) · Go · TypeScript/Node.js · Python  
**Trading:** CLOB APIs · WebSocket order book streaming · real-time event normalization · position sizing  
**Backend:** OAuth 2.0 · REST/WebSocket APIs · PostgreSQL · Redis · async workers  
**Infra:** GCP · AWS · Supabase

---

## Contact

**Web:** [yahyaehsan.dev](https://yahyaehsan.dev) · **Email:** yahyaehsan137@gmail.com · **Location:** Amsterdam
