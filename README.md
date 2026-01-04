# Yahya Ehsan

**Senior Systems Engineer | Rust Trading Bot Specialist**

Building high-performance, production-grade trading infrastructure for crypto traders and prediction markets. Specialized in sub-second latency systems, concurrent architectures, and real-time data processing.

**Currently:** Developing automated trading systems for Polymarket, DEX protocols, and prediction markets  
**Specialty:** High-performance systems programming in Rust with focus on concurrency and low-latency execution  
**Focus:** Arbitrage detection, market-making infrastructure, and distributed trading systems

---

## Featured Projects

### Polymarket Multi-Asset Trading Bot *(Private Client Work)*

High-performance trading infrastructure handling concurrent cryptocurrency markets (BTC, ETH, SOL, XRP) with sub-100ms event detection and execution latency.

**Architecture:**
- 4 independent asset executors running concurrently without blocking
- Round Transition Watcher for zero-delay round detection (<100ms)
- Order Book Watcher with WebSocket streaming, heartbeat monitoring, and reconnection logic
- Event normalization layer transforming raw market data into typed internal events
- Zero shared mutable state across await points for lock-free concurrency

**Stack:** Rust, Tokio async runtime, WebSockets, REST APIs  
**Delivered:** 72 hours from contract to production deployment  
**Status:** Currently running in production

---

### [Polymarket Event-Driven Trading Engine](https://github.com/yussypu/polymarket-engine) *(Open Source)*

Production-grade foundation for building Polymarket trading bots. Implements core infrastructure patterns: concurrent asset execution, real-time round detection, WebSocket order book streaming, and event-driven architecture.

**Technical Highlights:**
- Concurrent execution model with independent tasks per asset
- Sub-100ms round transition detection
- WebSocket connection management with automatic reconnection and state reconciliation
- Type-safe event normalization layer

**Stack:** Rust, Tokio, async/await, WebSocket protocols  
**Status:** Open source, actively maintained

---

### [Redis Clone - High-Performance Key-Value Store](https://github.com/yussypu/redis-rust)

Custom implementation of Redis core functionality in Rust, achieving 75M+ operations per second with concurrent client support.

**Features:**
- Multi-threaded architecture with lock-free data structures
- Support for core Redis commands (GET, SET, DEL, etc.)
- Custom RESP protocol parser
- Benchmarked performance metrics

**Stack:** Rust, concurrent data structures, network protocols  
**Performance:** 75M+ ops/sec on commodity hardware

---

### [HTTP Server - Ultra-Low Latency Web Server](https://github.com/yussypu/http-server-rust)

From-scratch HTTP/1.1 server implementation handling 93K+ requests per second with zero external dependencies.

**Features:**
- Custom HTTP parser and request handling
- Thread-per-connection model with efficient resource management
- Static file serving and routing
- Production-ready error handling

**Stack:** Pure Rust, TCP sockets, HTTP/1.1 protocol  
**Performance:** 93K+ req/sec sustained throughput

---

### Google Cloud Document Processing Pipeline *(Client Work)*

Built automated invoice parsing system using Google Vertex AI for extracting structured data from unstructured PDFs.

**Technical Highlights:**
- Google Cloud IAM authentication and service account integration
- Vertex AI API integration for document intelligence
- Structured data extraction with validation logic

**Stack:** Python, Google Cloud Vertex AI, IAM, service accounts  
**Status:** Delivered to client

---

### Lead Generation Automation Pipeline *(Client Work)*

Automated lead scraping and validation system for real estate/B2B clients with Google Sheets integration.

**Technical Highlights:**
- Email validation via SMTP verification
- Automated data cleaning and deduplication
- Google Sheets API integration for real-time updates
- Bypasses manual CSV imports with direct API writes

**Stack:** Python, Google Sheets API, SMTP protocols  
**Status:** Delivered to client

---

## Technical Expertise

**Systems Programming:**
- Rust (async/await, Tokio, performance optimization, lock-free concurrency)
- Low-level network programming (WebSockets, TCP/UDP, custom protocols)
- Concurrent and parallel system design
- Memory-safe systems with zero-cost abstractions

**Trading Infrastructure:**
- Real-time order book processing
- Market data normalization and aggregation
- Sub-millisecond latency optimization
- Event-driven architecture patterns

**Backend Engineering:**
- High-throughput API design and implementation
- Distributed systems and message passing
- OAuth 2.0 flows and token management
- Database design and optimization
- Cloud infrastructure (GCP, AWS)
- Background job processing (Cron, BullMQ)

**API Integration:**
- Google APIs (Calendar, Gmail, Sheets, Vertex AI)
- Financial data APIs (WebSocket/REST)
- Custom protocol implementations

**Secondary:**
- Python (data analysis, backtesting, AI/ML integration)
- TypeScript/JavaScript (full-stack development)
- SQL/NoSQL databases (PostgreSQL, Redis, Supabase)

---

## Open Source Contributions

Building tools and infrastructure for the trading and crypto communities:
- Production-ready trading bot frameworks
- High-performance systems programming examples
- Educational resources for systems-level Rust development

---

## Professional Experience

**Backend Engineer** @ Orbit Consulting (30 hrs/week)  
Building scalable backend systems and infrastructure

**Freelance Systems Engineer** @ Upwork  
Specialized in trading bot development, Google API integrations, and high-performance backend systems

**Computer Science** @ VU Amsterdam (3rd Year)  
Focus on distributed systems, algorithms, and high-performance computing

---

## Client Work

Available for custom trading bot development and backend infrastructure projects:
- Cross-platform arbitrage systems
- Market-making infrastructure
- Custom strategy automation
- High-performance API integrations
- Real-time data processing pipelines
- OAuth flows and secure token management

**Rates:** €3,500 standard bot development (72-hour delivery) | Custom quotes for complex systems

**Interested in working together?** → [yahyaehsan.dev](https://yahyaehsan.dev)

---

## Contact

- **Website:** [yahyaehsan.dev](https://yahyaehsan.dev)
- **Email:** yahyaehsan137@gmail.com
- **Location:** Amsterdam, Netherlands

---

*Building production-grade systems with Rust. Specializing in trading infrastructure that handles real money.*
