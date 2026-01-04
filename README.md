# Yahya Ehsan

**Senior Systems Engineer**

High-performance systems programming and production backend infrastructure. Rust for microsecond-latency trading systems, TypeScript/Node.js for secure API integrations and OAuth flows.

**Currently:** Building automated trading bots for Polymarket and prediction markets  
**Specialties:** Sub-second latency systems, concurrent architectures, OAuth/API integrations, real-time data processing

---

## Featured Projects


### [Polymarket Trading Bot Infrastructure](https://github.com/yussypu/polymarket-engine)

Production-grade foundation for building Polymarket trading bots. Concurrent asset execution, real-time market data streaming, event-driven architecture.

**Architecture:**
- 4 independent async executors (BTC, ETH, SOL, XRP) with isolated failure domains
- Sub-100ms round transition detection with dedicated watchers
- WebSocket order book streaming with heartbeat monitoring and auto-reconnection
- Event normalization layer (raw data → type-safe internal events)
- Zero shared mutable state across await points

**Stack:** Rust, Tokio async runtime, WebSockets, REST APIs  
**Performance:** Round detection <100ms, message processing <1ms, 10-20MB per asset

---

### Polymarket Multi-Asset Trading Bot *(Private Client Work)*

High-performance trading infrastructure handling concurrent cryptocurrency markets with sub-100ms event detection and execution latency.

**Delivered:** Full system from contract to production in 72 hours  
**Stack:** Rust, Tokio, WebSockets, REST APIs  
**Status:** Currently running in production for client

---

### [Google Calendar OAuth & Incremental Sync](https://github.com/yussypu/google-calendar-oauth-sync)

Clean implementation of Google Calendar's OAuth 2.0 flow with incremental sync using `nextSyncToken`. Demonstrates proper token management and efficient API usage patterns.

**Technical Highlights:**
- OAuth 2.0 with automatic token refresh (5min buffer before expiry)
- Incremental sync: first run fetches all, subsequent runs only fetch changes (10-100x faster)
- Encrypted token storage with AES-256-GCM
- Automatic recovery when sync tokens expire
- Rate limiting to avoid quota limits

**Stack:** TypeScript, Node.js, Google Calendar API, OAuth 2.0  
**Performance:** Full sync ~2-5s, incremental ~200-500ms (50 events)

---

### [Redis Clone](https://github.com/yussypu/redis-go)

In-memory key-value store in Go with thread-safe concurrent access. Demonstrates deep understanding of data structures and concurrency primitives.

**Technical Highlights:**
- `sync.RWMutex` for lock-free reads with multiple concurrent readers
- CLI and TCP server modes
- Custom benchmarking framework

**Performance:** SET 381ns/op, GET 16.8ns/op (Apple M1)  
**Stack:** Go, concurrent data structures, TCP networking

---

### [Real-Time File Sync Engine](https://github.com/yussypu/rust-file-sync)

High-performance file synchronization system with real-time change detection and end-to-end encryption.

**Technical Highlights:**
- Real-time file system monitoring with `notify` crate
- AES-256-GCM encryption for secure transfers
- Client-server architecture with async I/O

**Performance:** 123µs average sync time per file (5000+ files)  
**Stack:** Rust, Tokio, AES encryption, async file I/O

---

### [RISC-V Operating System Kernel](https://github.com/yussypu/riscv-kernel)

Educational OS kernel implementing virtual memory, process management, and context switching on RISC-V architecture.

**Technical Highlights:**
- Two-level page tables (SV32) with virtual-to-physical translation
- Process control blocks with state tracking
- Context switching with register preservation and stack swapping
- Inline assembly for low-level CSR manipulation

**Stack:** Rust, RISC-V assembly, bare-metal systems programming

---

## Technical Expertise

**Systems Programming:**
- Rust (async/await, Tokio, lock-free concurrency, zero-cost abstractions)
- Go (concurrent patterns, sync primitives)
- Low-level network programming (WebSockets, TCP/UDP, custom protocols)
- Memory-safe systems with performance optimization

**Backend & APIs:**
- OAuth 2.0 flows with automatic token refresh and secure storage
- Google APIs (Calendar, Gmail, Sheets, Vertex AI, Cloud IAM)
- RESTful API design and WebSocket streaming
- Background job processing (Cron, BullMQ, async workers)
- TypeScript/Node.js for production backend services

**Trading Infrastructure:**
- Real-time order book processing
- Market data normalization and event-driven architecture
- Sub-millisecond latency optimization
- Concurrent execution models with isolated failure domains

**Other:**
- Python (data processing, AI/ML integration, automation)
- Cloud platforms (GCP, AWS, Supabase)
- Database design (PostgreSQL, Redis)

---

## Professional Experience

**Backend Engineer** @ Orbit Consulting (30 hrs/week)  
Building scalable backend systems and infrastructure

**Freelance Systems Engineer** @ Upwork  
Specialized in trading bot development, Google API integrations, and high-performance backend systems

---

## Client Work

Available for:
- **Trading bots:** High-performance Rust systems for crypto/prediction markets
- **API integrations:** Google Calendar/Gmail/Sheets with OAuth flows and secure token management
- **Backend infrastructure:** Real-time data processing, WebSocket systems, async workers
- **Systems programming:** Low-latency systems, concurrent architectures

**Standard bot development:** €3,500 (72-hour delivery)  
**Complex systems:** Custom quotes for multi-platform infrastructure, fund management systems (€5,000-€15,000)

**Interested in working together?** → [yahyaehsan.dev](https://yahyaehsan.dev)

---

## Contact

- **Website:** [yahyaehsan.dev](https://yahyaehsan.dev)
- **Email:** yahyaehsan137@gmail.com
- **Location:** Amsterdam, Netherlands

---

*Production-grade systems - from microsecond-latency trading infrastructure to secure OAuth integrations.*
