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

**dune**

[ocaml/dune#15017](https://github.com/ocaml/dune/pull/15017). cram's path tokenizer split at the first space, so a project path containing one left the absolute prefix unsanitized; fix matches the build path prefix map sources literally.

[ocaml/dune#15016](https://github.com/ocaml/dune/pull/15016). under --error-reporting=twice the deterministic error list ran into build output with nothing marking its start; added a separator before it, suppressed when there are no errors.



**mistral.rs** 

[EricLBuehler/mistral.rs#2170](https://github.com/EricLBuehler/mistral.rs/pull/2170). traced an engine panic to an unwrap on a best effort send that fired when a client disconnected mid request.

### contact
yahyaehsan.dev · yahyaehsan137@gmail.com · Amsterdam
