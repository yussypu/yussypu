I write Rust and C++, mostly low level systems where correctness and latency pull against each other.
I like measuring exactly what that costs.

### now
C++ EVM log parser at a DeFi terminal. Multi chain, real time. Single producer WebSocket ingestion, tx level worker parallelism, SPMC queue.

### before
Quant research and the Rust execution stack under it, on Polymarket. Sub 100ms market-state detection, isolated failure domains, kill switch.


selected projects

[crackeddb](https://github.com/yussypu/crackeddb): embedded OLTP engine. Serializable; SSI specified in TLA+ and machine checked; every source of nondeterminism behind one trait, so a bug from a seed reproduces byte for byte. The only backend in its own benchmark that detects write skew. The mature engines are faster and commit the anomaly.

[gavel](https://github.com/yussypu/gavel): single threaded exchange matching engine in C++23. The sequenced input stream determines every output byte; the output hash comes back bit identical across O0, O2 and O3. Checked against a real NASDAQ trading day, about 91,700 executions, zero displayed price priority violations. p50 around 83 ns.

[vincr](https://github.com/yussypu/vincr): the propagation algorithm under Jane Street's Incremental, modeled in Lean 4 and proved consistent with zero sorry, then differential tested against janestreet/incremental. Verified work in this space proves the update functions and leaves the engine, where the bugs actually live, outside the proof. These proofs are engine level.

[deja](https://github.com/yussypu/deja): record, replay and statistically compare LLM agent trajectories. rr for agents, with error bars. On a 26 task Claude Code benchmark, eyeballing the mean delta calls a false winner 60% of the time comparing an agent against itself; a correct paired test holds it to 2.8%. Replays a session with the network dead and localizes any divergence to the exact field that moved.

[apex](https://github.com/yussypu/apex): minimum lap time simulator and racing line optimiser, every number checkable against closed form physics. Calibrated to Verstappen's 2023 Austrian pole lap it predicts 64.69 s against a real 64.39 s. The solver is differentiable in JAX, so it rediscovers real F1 setup practice on its own: minimum wing at Monza, maximum at the Hungaroring.

[stopwatch](https://github.com/yussypu/stopwatch): recovering a sub nanosecond duration from a 24 MHz clock that cannot see one.

[binding-ladder](https://github.com/yussypu/binding-ladder): measuring what it costs to push an invariant from a comment down to "wont compile." Compile time grows roughly quadratically; runtime stays at zero.

Also: urduclang (write C in Urdu script), c-os (RISC-V kernel), rust-file-sync.

### open source

**dune**

[ocaml/dune#15017](https://github.com/ocaml/dune/pull/15017). cram's path tokenizer split at the first space, so a project path containing one left the absolute prefix unsanitized; fix matches the build path prefix map sources literally.

[ocaml/dune#15016](https://github.com/ocaml/dune/pull/15016). under --error-reporting=twice the deterministic error list ran into build output with nothing marking its start; added a separator before it, suppressed when there are no errors.



**mistral.rs** 

[EricLBuehler/mistral.rs#2170](https://github.com/EricLBuehler/mistral.rs/pull/2170). traced an engine panic to an unwrap on a best effort send that fired when a client disconnected mid request.

### contact
yahyaehsan.dev · yahyaehsan137@gmail.com · Amsterdam
