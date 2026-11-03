| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# 你好，我是马库斯·万斯（Marcus Vance） 👋

专注于**低延迟网络**、**嵌入式存储引擎**与**分布式共识算法**的系统软件工程师。

致力于设计和构建具有硬件同理心（Mechanical Sympathy）、零内存分配网络协议以及确定性崩溃恢复机制的高效基础设施。坚信软件在默认状态下应当快速、极简且具备高度可观测性。

---

## 🔭 进行中的核心开源项目

| 项目名称 | 开发语言 | 架构特点与核心目标 | 当前状态 |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | 零拷贝、写入优化的 LSM-Tree 嵌入式存储引擎，支持并发 Memtable、分层压缩（Tiered Compaction）与 Direct I/O WAL。 | 核心引擎 v0.8.2 |
| **raft-ring** | Go | 极简 Raft 分布式共识实现，配备可插拔传输层（QUIC / gRPC）与基于 SWIK 的 Gossip 节点成员发现机制。 | 积极迭代中 |
| **wire-bench** | C++20 | 基于 Linux `io_uring` 与 eBPF 跟踪点的微秒级网络套接字基准测试套件，精准分析 TCP/UDP 尾部延迟。 | 稳定版本 v1.2.0 |
| **kflow** | Go | 终端原生 TUI 监控工具，用于实时观测 Kafka 分区流量分布、重平衡事件及消费者堆积延迟。 | 开源发布 |

---

## 🛠️ 技术栈与工具库

| 领域分类 | 主要技术与核心工具 |
| :--- | :--- |
| **编程语言** | Rust, Go, C++20, C, Zig, Python (辅助工具), Bash |
| **存储与数据** | LSM-Trees, B-Trees, RocksDB 内部机制, PostgreSQL, Redis, Apache Kafka |
| **系统与底层优化** | Linux 系统级编程, `io_uring`, epoll, eBPF, SIMD 向量化优化, 缓存行对齐 |
| **并发与共识机制** | Raft, Paxos, 无锁环形缓冲区 (Lock-free Ring Buffer), MPMC 队列 |
| **可观测性与性能剖析**| Linux `perf`, 火焰图 (Flamegraphs), Valgrind, LLDB, eBPF Tracepoints |
| **开发环境与工具** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 工程设计准则

- **硬件协同优先 (Mechanical Sympathy)**：在着手优化代码前，务必深入理解内存层级结构、CPU 缓存行边界以及分支预测器的物理特性。
- **基准测试胜于凭空假设**：“除上帝之外，其余一切皆须凭可复现的微基准测试与火焰图来证明。”
- **面向崩溃的设计 (Crash-Only Design)**：任何存储系统都必须具备在任意机器指令执行时遭遇突然断电或 SIGKILL 信号后安全无损自愈的能力。
- **杜绝冗余依赖**：最稳健的第三方库正是你从未引入的那一个。时刻保持依赖关系图轻量、可审查且具备高抗风险能力。

---

## 📈 近期开发动向

```text
当前迭代周期:
  [■■■■■■■■■□] 90% - 将 vortex-db WAL 刷盘链路迁移至异步 io_uring 架构
  [■■■■■■□□□□] 60% - 实现 raft-ring 快照状态机传输管道
  [■■■■■■■■■■] 100% - 正式发布面向 Linux 6.8+ 的 wire-bench 延迟剖析套件
```

---

## 📬 联系方式与主页

- **电子邮箱**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **时区**: UTC+9 / 长期参与全球分布式远程开源协同
