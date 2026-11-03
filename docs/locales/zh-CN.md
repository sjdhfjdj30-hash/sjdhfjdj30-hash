| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# 你好，我是资深系统工程师 Marcus Vance 👋

专注于**低延迟网络通信**、**嵌入式存储引擎**与**分布式共识协议**的资深系统软件工程师。

我致力于设计确定性、内存高效的基础设施，尤其注重机械共鸣（Mechanical Sympathy）、零内存分配网络协议以及确定性的崩溃恢复语义。我认为优质软件应当天生具备极致速度、透明可观测性与坚固的容错能力。

---

## 🔭 核心工程项目

| 项目 | 语言 | 架构与核心定位 | 状态 |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | 支持并发 Memtable、分层压缩（Tiered Compaction）与 Direct I/O WAL 的零拷贝写优化 LSM-Tree 嵌入式存储引擎 | 核心引擎 v0.8.2 |
| **raft-ring** | Go | 具备可插拔传输层（QUIC / gRPC）与 SWIK Gossip 成员发现的高性能 Raft 分布式共识库 | 积极迭代中 |
| **wire-bench** | C++20 | 基于 Linux `io_uring` 与 eBPF 跟踪点的微秒级套接字基准测试工具，精准分析 TCP/UDP 长尾延迟 | 稳定版 v1.2.0 |
| **kflow** | Go | 实时追踪 Kafka 分区流量、再平衡事件与消费者堆积的终端原生 TUI 仪表板 | 开源发布 |

---

## 🛠️ 技术栈与工具箱

| 领域 | 核心技术与工具 |
| :--- | :--- |
| **编程语言** | Rust, Go, C++20, C, Zig, Python (内部工具), Bash |
| **存储与数据引擎** | LSM-Trees, B-Trees, RocksDB 内核, PostgreSQL, Redis, Apache Kafka |
| **系统与底层优化** | Linux 系统编程, `io_uring`, epoll, eBPF, SIMD 向量化, 缓存行对齐 |
| **并发与分布式共识**| Raft, Paxos, 无锁环形缓冲区（Lock-free Ring Buffer）, MPMC 队列 |
| **可观测性与性能分析**| Linux `perf`, 火焰图（Flamegraphs）, Valgrind, LLDB, eBPF Tracepoints |
| **工作环境** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 工程设计哲学

- **机械共鸣优先 (Mechanical Sympathy)**: 在着手优化代码前，必须深入理解物理内存层级、CPU 缓存行边界与分支预测器的底层机理。
- **基准测试优于主观推断**: “除了上帝，其余一切都必须用可复现的微基准测试与火焰图来证明。”
- **面向崩溃设计 (Crash-Only Design)**: 任何存储系统都必须能在任意指令执行中突发掉电或遭遇 SIGKILL 时，完整保留数据一致性并干净恢复。
- **克制外部依赖**: 最健壮的第三方依赖就是未曾引入的依赖。保持依赖图极简、透明且可审计。

---

## 📈 当前工程焦点

```text
当前迭代周期:
  [■■■■■■■■■□] 90% - 将 vortex-db WAL 刷盘路径重构为异步 io_uring
  [■■■■■■□□□□] 60% - 在 raft-ring 中实现快照状态机传输协议
  [■■■■■■■■■■] 100% - 发布兼容 Linux 6.8+ 的 wire-bench 延迟剖析套件
```

---

## 📬 联系方式与链接

- **Email**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **时区**: UTC+9 / 积极参与全球分布式开源项目协作
