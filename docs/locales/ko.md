| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# 안녕하세요, 시니어 시스템 엔지니어 마커스 반스(Marcus Vance)입니다 👋

**초저지연 네트워크 통신**, **임베디드 스토리지 엔진**, 그리고 **분산 합의 프로토콜**을 전문으로 연구하고 설계하는 시니어 시스템 소프트웨어 엔지니어입니다.

하드웨어 친화적 아키텍처(Mechanical Sympathy), 무할당(Zero-allocation) 네트워크 프로토콜, 그리고 비정상 종료 시에도 안전한 크래시 복구(Crash-recovery) 메커니즘을 중점으로 견고한 고성능 인프라를 구축합니다. 소프트웨어는 기본적으로 빠르고, 명확하며, 제1원리(First-principles)에 의해 결함에 견고해야 한다고 믿습니다.

---

## 🔭 핵심 엔지니어링 프로젝트

| 프로젝트 | 언어 | 아키텍처 및 핵심 목적 | 진행 상태 |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | 동시성 멤테이블(Memtable), 계층형 컴팩션(Tiered Compaction), Direct I/O WAL을 지원하는 제로카피 쓰기 최적화 LSM-Tree 임베디드 스토리지 엔진 | 코어 엔진 v0.8.2 |
| **raft-ring** | Go | 플러그형 전송 계층(QUIC / gRPC)과 SWIK 기반 가십 멤버십 탐색을 탑재한 고성능 Raft 분산 합의 알고리즘 라이브러리 | 활발히 개발 중 |
| **wire-bench** | C++20 | Linux `io_uring` 및 eBPF 트레이스포인트를 활용하여 TCP/UDP 테일 레이턴시(Tail Latency)를 마이크로초 단위로 정밀 측정하는 소켓 벤치마크 툴킷 | 안정화 버전 v1.2.0 |
| **kflow** | Go | Kafka 파티션 트래픽, 리밸런싱 이벤트, 컨슈머 랙(Lag)을 실시간으로 추적하는 터미널 네이티브 TUI 대시보드 | 오픈소스 공개 |

---

## 🛠️ 기술 스택 및 개발 툴킷

| 분류 | 주요 기술 및 도구 |
| :--- | :--- |
| **프로그래밍 언어** | Rust, Go, C++20, C, Zig, Python (내부 도구), Bash |
| **스토리지 및 데이터** | LSM-Trees, B-Trees, RocksDB 인터널, PostgreSQL, Redis, Apache Kafka |
| **시스템 및 저수준 최적화** | Linux 시스템 프로그래밍, `io_uring`, epoll, eBPF, SIMD 연산, 캐시 라인 정렬 |
| **동시성 및 합의 알고리즘**| Raft, Paxos, 락프리 링 버퍼(Lock-free Ring Buffer), MPMC 큐 |
| **관측성 및 프로파일링** | Linux `perf`, 플레임그래프(Flamegraph), Valgrind, LLDB, eBPF Tracepoints |
| **작업 환경 및 도구** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 엔지니어링 철학

- **하드웨어 친화적 설계(Mechanical Sympathy)**: 코드를 최적화하기 전에 메모리 계층 구조, CPU 캐시 라인 경계, 분기 예측기(Branch Predictor)의 물리적 동작 원리를 먼저 이해합니다.
- **가정 대신 벤치마크**: "우리가 믿는 것은 신뿐이며, 그 외의 모든 것은 재현 가능한 마이크로 벤치마크와 플레임그래프로 증명되어야 한다."
- **크래시 전제 설계(Crash-Only Design)**: 모든 스토리지 시스템은 임의의 명령어 실행 도중 갑작스러운 전원 차단이나 SIGKILL이 발생하더라도 데이터 무결성을 유지하며 깨끗하게 복구되어야 합니다.
- **최소 의존성 유지**: 최고의 라이브러리 의존성은 아예 추가하지 않은 의존성입니다. 의존성 트리를 콤팩트하고 견고하게 유지합니다.

---

## 📈 최근 개발 집중 분야

```text
현재 스프린트:
  [■■■■■■■■■□] 90% - vortex-db WAL 플러시 경로의 비동기 io_uring 전환
  [■■■■■■□□□□] 60% - raft-ring 스냅샷 상태 머신 전송 파이프라인 구현
  [■■■■■■■■■■] 100% - Linux 6.8+ 대응 wire-bench 지연시간 프로파일러 릴리스
```

---

## 📬 연락처 및 채널

- **이메일**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **시간대**: UTC+9 / 전 세계 분산 원격 오픈소스 협업 참여 중
