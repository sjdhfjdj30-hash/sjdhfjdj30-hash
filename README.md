| [KR 한국어](./docs/locales/ko.md) | [US English](./README.md) | [JP 日本語](./docs/locales/ja.md) | [CN 简体中文](./docs/locales/zh-CN.md) | [ES Español](./docs/locales/es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./docs/locales/fr.md) | [DE Deutsch](./docs/locales/de.md) | [RU Русский](./docs/locales/ru.md) | [BR Português](./docs/locales/pt-BR.md) | [SA العربية](./docs/locales/ar.md) |

---

# Hi there, I'm Marcus Vance 👋

Systems Software Engineer focused on **low-latency networking**, **embedded storage engines**, and **distributed consensus algorithms**.

I build deterministic, memory-efficient infrastructure with an emphasis on mechanical sympathy, zero-allocation network protocols, and robust crash-recovery semantics. I believe software should be fast, simple, and observable by default.

---

## 🔭 Active Work & Projects

| Project | Language | Architecture & Purpose | Status |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Zero-copy, write-optimized LSM-tree embedded storage engine featuring concurrent memtables, tiered compaction, and direct I/O WAL. | Core Engine v0.8.2 |
| **raft-ring** | Go | Minimalist Raft consensus implementation with pluggable transport layers (QUIC / gRPC) and SWIK gossip membership discovery. | Active Development |
| **wire-bench** | C++20 | Microsecond-precision socket benchmark suite testing TCP/UDP tail latencies using Linux `io_uring` and eBPF tracepoints. | Stable v1.2.0 |
| **kflow** | Go | Terminal-native TUI monitoring tool for real-time Kafka partition traffic, rebalance events, and consumer lag tracking. | Open Source |

---

## 🛠️ Technical Stack & Toolkit

| Category | Primary Technologies & Tooling |
| :--- | :--- |
| **Languages** | Rust, Go, C++20, C, Zig, Python (Tooling), Bash |
| **Storage & Engines** | LSM-Trees, B-Trees, RocksDB internals, PostgreSQL, Redis, Apache Kafka |
| **Systems & Low-Level** | Linux Systems Programming, `io_uring`, epoll, eBPF, SIMD optimizations, Cache-line alignment |
| **Concurrency & Consensus**| Raft, Paxos, Lock-free Ring Buffers, Multi-Producer Multi-Consumer (MPMC) Queues |
| **Observability & Profiling**| Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints, OpenTelemetry |
| **Workflow & Environment** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Engineering Principles

- **Mechanical Sympathy First**: Understand the memory hierarchy, cache line boundaries, and branch predictors before optimizing code.
- **Benchmarks Over Assumptions**: "In God we trust; all others bring reproducible microbenchmarks and flamegraphs."
- **Crash-Only Design**: Every storage system must be capable of recovering cleanly from an abrupt power loss or SIGKILL at any arbitrary instruction.
- **Minimal Dependencies**: The best dependency is the one you never added. Keep the dependency graph tight, auditable, and resilient.

---

## 📈 Recent Activity & Workflows

```text
Current Sprint:
  [■■■■■■■■■□] 90% - Porting vortex-db WAL flush path to asynchronous io_uring
  [■■■■■■□□□□] 60% - Implementing snapshot state machine transfers in raft-ring
  [■■■■■■■■■■] 100% - Release wire-bench latency profiling runner for Linux 6.8+
```

---

## 📬 Contact & Links

- **Email**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Timezone**: UTC+9 / Available for distributed open-source collaboration worldwide
