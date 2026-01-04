# Yahya Ehsan

**Senior Systems Engineer**

Building high-performance production systems across the stack - from sub-millisecond trading infrastructure in Rust to secure API integrations and backend services in TypeScript/Node.js.

**Specialties:** High-performance systems programming, real-time data processing, OAuth/API integrations, distributed architectures

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

### [Google Calendar Incremental Sync Engine](https://github.com/yussypu/google-calendar-sync) *(Open Source)*

Production-ready implementation of Google Calendar OAuth flow and incremental sync using nextSyncToken pattern. Demonstrates secure token management and efficient API usage.

**Technical Highlights:**
- Complete OAuth 2.0 flow with automatic token refresh
- Incremental sync: first run fetches full data, subsequent runs only fetch changes
- Token rotation middleware with expiry detection
- TypeScript with full type safety
- Clean error handling and reconnection logic

**Stack:** TypeScript, Node.js, Google Calendar API, OAuth 2.0  
**Status:** Open source, documented demo

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

**Languages & Frameworks:**
- **Rust:** async/await, Tokio, lock-free concurrency, performance optimization
- **TypeScript/JavaScript:** Node.js, Express, React, async patterns
- **Python:** Data processing, AI/ML integration, automation

**Backend & APIs:**
- OAuth 2.0 flows and secure token management
- Google APIs (Calendar, Gmail, Sheets, Vertex AI, Cloud IAM)
- RESTful API design and implementation
- WebSocket protocols and real-time data streaming
- Background job processing (Cron, BullMQ, async workers)

**Systems & Infrastructure:**
- Low-level network programming (TCP/UDP, custom protocols)
- Concurrent and parallel system design
- Event-driven architecture patterns
- Cloud platforms (GCP, AWS, Supabase)
- Database design (PostgreSQL, Redis, Supabase)

**Trading & Finance:**
- Real-time order book processing
- Market data normalization and aggregation
- Sub-millisecond latency optimization
- High-frequency trading infrastructure

---

## Open Source Contributions

Building tools and infrastructure for developers and traders:
- Production-ready trading bot frameworks (Rust)
- API integration patterns and best practices (TypeScript/Node.js)
- High-performance systems programming examples
- Educational resources for distributed systems

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

Available for:
- Trading bot development (Rust, high-performance systems)
- Google API integrations (Calendar, Gmail, Sheets, OAuth flows)
- Backend infrastructure and API development
- Real-time data processing pipelines
- Secure authentication and token management systems

**Rates:** €3,500 standard bot development (72-hour delivery) | Custom quotes for complex systems

**Interested in working together?** → [yahyaehsan.dev](https://yahyaehsan.dev)

---

## Contact

- **Website:** [yahyaehsan.dev](https://yahyaehsan.dev)
- **Email:** yahyaehsan137@gmail.com
- **Location:** Amsterdam, Netherlands

---

*Building production-grade systems - from microsecond-latency trading infrastructure in Rust to secure OAuth flows in TypeScript.*
