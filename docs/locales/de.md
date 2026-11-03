| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Hallo, ich bin Marcus Vance 👋

Systemsoftware-Entwickler mit Schwerpunkt auf **extrem latenzarmen Netzwerken**, **eingebetteten Speicher-Engines** und **verteilten Konsensalgorithmen**.

Ich entwerfe und baue deterministische, speichereffiziente Infrastrukturen mit starkem Fokus auf mechanische Sympathie (Mechanical Sympathy), allokationsfreie Netzwerkprotokolle und ausfallsichere Wiederherstellungssemantiken. Ich bin davon überzeugt, dass Software standardmäßig schnell, einfach und beobachtbar sein muss.

---

## 🔭 Aktuelle Projekte & Open Source

| Projekt | Sprache | Architektur & Zielsetzung | Status |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Zero-Copy, schreiboptimierte eingebettete LSM-Tree-Speicher-Engine mit nebenläufigen Memtables, gestufter Kompaktierung und Direct-I/O-WAL. | Kern-Engine v0.8.2 |
| **raft-ring** | Go | Minimalistische Raft-Konsens-Implementierung mit austauschbaren Transportschichten (QUIC / gRPC) und SWIK-Gossip-Mitgliedschaftserkennung. | Aktive Entwicklung |
| **wire-bench** | C++20 | Mikrosekunden-genaue Socket-Benchmark-Suite zur Messung von TCP/UDP-Tail-Latenzen mittels Linux `io_uring` und eBPF-Tracepoints. | Stabile Version v1.2.0 |
| **kflow** | Go | Terminal-natives TUI-Dashboard zur Echtzeit-Überwachung von Kafka-Partitionsverkehr, Rebalance-Ereignissen und Consumer-Lag. | Open Source |

---

## 🛠️ Technologie-Stack & Werkzeuge

| Kategorie | Bevorzugte Technologien & Tools |
| :--- | :--- |
| **Programmiersprachen** | Rust, Go, C++20, C, Zig, Python (Tools), Bash |
| **Speicher & Daten** | LSM-Trees, B-Trees, RocksDB-Interna, PostgreSQL, Redis, Apache Kafka |
| **System- & Low-Level-Optimierung** | Linux-Systemprogrammierung, `io_uring`, epoll, eBPF, SIMD-Optimierung, Cache-Line-Ausrichtung |
| **Nebenläufigkeit & Konsens** | Raft, Paxos, sperrenfreie Ringpuffer (Lock-free Ring Buffers), MPMC-Warteschlangen |
| **Beobachtbarkeit & Profiling** | Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF-Tracepoints, OpenTelemetry |
| **Arbeitsumgebung** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux-Kernel 6.x |

---

## 📐 Technische Prinzipien

- **Mechanische Sympathie zuerst**: Verstehe die Speicherhierarchie, CPU-Cache-Line-Grenzen und Sprungvorhersagen (Branch Predictors), bevor du versuchst, Code zu optimieren.
- **Benchmarks vor Vermutungen**: „Auf Gott vertrauen wir; alle anderen müssen reproduzierbare Mikrobenchmarks und Flamegraphs vorlegen.“
- **Crash-Only-Architektur**: Jedes Speichersystem muss in der Lage sein, sich nach einem plötzlichen Stromausfall oder einem SIGKILL-Signal bei jedem beliebigen Befehl sauber und ohne Datenverlust zu erholen.
- **Minimale Abhängigkeiten**: Die beste Abhängigkeit ist diejenige, die du gar nicht erst hinzugefügt hast. Halte den Abhängigkeitsbaum straff, überprüfbar und widerstandsfähig.

---

## 📈 Aktuelle Entwicklungsschritte

```text
Aktueller Sprint:
  [■■■■■■■■■□] 90% - Portierung des vortex-db WAL-Flush-Pfads auf asynchrones io_uring
  [■■■■■■□□□□] 60% - Implementierung des Snapshot-State-Machine-Transfers in raft-ring
  [■■■■■■■■■■] 100% - Release des wire-bench Latenzprofilers für Linux 6.8+
```

---

## 📬 Kontakt & Links

- **E-Mail**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Zeitzone**: UTC+9 / Offen für weltweite verteilte Open-Source-Zusammenarbeit
