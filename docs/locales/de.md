| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# Hallo, ich bin Marcus Vance 👋

Senior Systems Software Engineer mit Fokus auf **extrem latenzarme Netzwerke**, **eingebettete Storage-Engines** und **verteilte Konsensprotokolle**.

Ich entwickle deterministische, speichereffiziente Infrastruktur mit kompromisslosem Fokus auf Hardware-Verständnis (Mechanical Sympathy), allokationsfreie Netzwerkprotokolle und verlässliche Crash-Recovery-Semantik. Ich bin überzeugt, dass Software von Grund auf schnell, transparent und fehlerresistent sein muss.

---

## 🔭 Zentrale Entwicklungsprojekte

| Projekt | Sprache | Architektur & Fokus | Status |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Zero-Copy, schreiboptimierte LSM-Tree Embedded Storage Engine mit nebenläufigen Memtables, gestufter Kompaktierung und Direct I/O WAL. | Core Engine v0.8.2 |
| **raft-ring** | Go | Hochperformante Raft-Konsensisierung mit austauschbaren Transportschichten (QUIC / gRPC) und SWIK-Gossip-Mitgliedschaftserkennung. | Aktive Entwicklung |
| **wire-bench** | C++20 | Mikrosekunden-präzise Socket-Benchmark-Suite zur Profilierung von TCP/UDP-Tail-Latenzen mittels Linux `io_uring` und eBPF-Tracepoints. | Stabile Version v1.2.0 |
| **kflow** | Go | Terminal-natives TUI-Monitoring-Tool zur Echtzeit-Analyse von Kafka-Partition-Traffic, Rebalance-Events und Consumer-Lag. | Open Source |

---

## 🛠️ Tech-Stack & Werkzeuge

| Kategorie | Primäre Technologien |
| :--- | :--- |
| **Programmiersprachen** | Rust, Go, C++20, C, Zig, Python (Tools), Bash |
| **Storage & Engines** | LSM-Trees, B-Trees, RocksDB Internals, PostgreSQL, Redis, Apache Kafka |
| **System- & Low-Level** | Linux Systemprogrammierung, `io_uring`, epoll, eBPF, SIMD-Optimierung, Cache-Line-Alignment |
| **Parallelität & Konsens** | Raft, Paxos, Lock-free Ringbuffer, MPMC-Warteschlangen |
| **Observability & Profiling**| Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints |
| **Arbeitsumgebung** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Entwicklungsphilosophie

- **Hardware-Verständnis an erster Stelle (Mechanical Sympathy)**: Verstehe die Speicherhierarchie, Cache-Line-Grenzen und Sprungvorhersagen (Branch Predictors), bevor du Code optimierst.
- **Messung statt Vermutung**: „Auf Gott vertrauen wir; alle anderen müssen reproduzierbare Mikro-Benchmarks und Flamegraphs vorlegen.“
- **Crash-Only-Design**: Jedes Speichersystem muss nach einem plötzlichen Stromausfall oder SIGKILL bei jedem beliebigen Befehl sauber und konsistent wieder anlaufen können.
- **Minimale Abhängigkeiten**: Die beste Abhängigkeit ist die, die man gar nicht erst hinzugefügt hat. Den Abhängigkeitsgraphen schlank, auditierbar und robust halten.

---

## 📈 Aktueller Entwicklungsschwerpunkt

```text
Aktueller Sprint:
  [■■■■■■■■■□] 90% - Portierung des vortex-db WAL-Flush-Pfads auf asynchrones io_uring
  [■■■■■■□□□□] 60% - Implementierung von Snapshot-Zustandsmaschinen-Transfers in raft-ring
  [■■■■■■■■■■] 100% - Release des wire-bench Latenzprofilers für Linux 6.8+
```

---

## 📬 Kontakt & Links

- **E-Mail**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Zeitzone**: UTC+9 / Offen für weltweite verteilt-asynchrone Open-Source-Zusammenarbeit
