I write Rust and C++, mostly low level systems where correctness and latency pull against each other.
I like measuring exactly what that costs.

### now
C++ EVM log parser at a DeFi terminal. Multi chain, real time. Single producer WebSocket ingestion, tx level worker parallelism, SPMC queue.

### before
Quant research and the Rust execution stack under it, on Polymarket. Sub 100ms market-state detection, isolated failure domains, kill switch.


### selected projects
**crackeddb**: embedded OLTP engine. Serializable; SSI specified in TLA+ and machine checked; every source of nondeterminism behind one trait, so a bug from a seed reproduces byte for byte. The only backend in its own benchmark that detects write skew. The mature engines are faster and commit the anomaly.

**stopwatch**: recovering a sub nanosecond duration from a 24 MHz clock that cannot see one.

**binding-ladder**: measuring what it costs to push an invariant from a comment down to "wont compile." Compile time grows roughly quadratically; runtime stays at zero.

**Also**: urduclang (write C in Urdu script), c-os (RISC-V kernel), rust-file-sync.

### open source
mistral.rs: https://github.com/EricLBuehler/mistral.rs/pull/2170. traced an engine panic to an unwrap on a best effort send that fired when a client disconnected mid request.


yahyaehsan.dev · yahyaehsan137@gmail.com · Amsterdam
