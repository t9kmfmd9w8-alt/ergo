Ergo — Distributed Actor Framework for Go

Build fault-tolerant, distributed systems in Go without managing the complexity of distributed systems yourself.

Ergo is a high-performance actor framework for Go, inspired by Erlang/OTP. It provides the building blocks for developing concurrent, fault-tolerant, and distributed applications using isolated processes, asynchronous message passing, and automatic supervision.

Instead of coordinating shared state with mutexes, managing goroutine lifecycles, implementing failure recovery, and building custom networking infrastructure, Ergo gives you a unified programming model for both local concurrency and distributed execution.

Actors communicate through messages, processes are isolated, failures are handled through supervision trees, and every process can be addressed across the cluster using the same API.

One programming model. From a single node to a distributed cluster.

* Concurrency without shared-state synchronization: Processes handle messages sequentially, eliminating data races on actor-owned state.
* Automatic fault recovery: Supervision trees monitor processes and apply configurable restart strategies.
* Transparent distribution: Communicate with local and remote processes through the same interface.
* Built-in distributed infrastructure: Service discovery, networking, event distribution, remote process spawning, and cluster orchestration.
* Production observability: Inspect processes, monitor cluster health, analyze performance, and trace messages across nodes.
* AI-native operations: Expose running clusters through MCP, allowing AI assistants to inspect and diagnose distributed applications.

Inspired by Erlang/OTP. Written in pure Go. Zero external dependencies.