| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Olá, eu sou Marcus Vance 👋

Engenheiro de software de sistemas especializado em **redes de ultra-baixa latência**, **motores de armazenamento embarcados** e **algoritmos de consenso distribuído**.

Projeto e construo infraestruturas determinísticas e com uso eficiente de memória, com foco em simpatia mecânica (Mechanical Sympathy), protocolos de rede sem alocação intermediária (zero-allocation) e resiliência garantida contra falhas repentinas. Acredito que o software deve ser naturalmente rápido, enxuto e observável por padrão.

---

## 🔭 Projetos em andamento e Open Source

| Projeto | Linguagem | Arquitetura e objetivo | Status |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Motor de armazenamento LSM-tree embutido com zero-copy otimizado para escrita, contendo memtables concorrentes, compactação escalonada e WAL com Direct I/O. | Motor principal v0.8.2 |
| **raft-ring** | Go | Implementação minimalista do consenso Raft com camadas de transporte modulares (QUIC / gRPC) e descoberta de nós via protocolo Gossip (SWIK). | Em desenvolvimento ativo |
| **wire-bench** | C++20 | Suite de benchmarks de sockets com precisão em microssegundos para análise de latências de cauda TCP/UDP utilizando `io_uring` e tracepoints eBPF. | Versão estável v1.2.0 |
| **kflow** | Go | Painel TUI nativo para terminal para monitoramento em tempo real do tráfego de partições Kafka, rebalanceamentos e lag de consumidores. | Código aberto |

---

## 🛠️ Stack técnica e ferramentas

| Categoria | Tecnologias e ferramentas principais |
| :--- | :--- |
| **Linguagens** | Rust, Go, C++20, C, Zig, Python (ferramentas auxiliares), Bash |
| **Armazenamento & Dados** | LSM-Trees, B-Trees, arquitetura interna do RocksDB, PostgreSQL, Redis, Apache Kafka |
| **Sistemas & Otimização de Baixo Nível** | Programação de sistemas Linux, `io_uring`, epoll, eBPF, instruções SIMD, alinhamento de cache-line |
| **Concorrência & Consenso** | Raft, Paxos, buffers circulares sem travas (lock-free ring buffers), filas MPMC |
| **Observabilidade & Profiling** | Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints, OpenTelemetry |
| **Ambiente de Trabalho** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Princípios de engenharia

- **Simpatia mecânica em primeiro lugar**: Entenda a hierarquia de memória, os limites das linhas de cache da CPU e o funcionamento dos preditores de desvio antes de tentar otimizar qualquer código.
- **Métricas superam suposições**: "Em Deus nós confiamos; todos os outros devem trazer microbenchmarks reproduzíveis e flamegraphs."
- **Design preparado para falhas (Crash-Only)**: Todo motor de armazenamento deve ser capaz de se recuperar perfeitamente e sem corrupção após uma queda abrupta de energia ou um sinal SIGKILL em qualquer instrução.
- **Mínimo de dependências**: A melhor dependência é aquela que você nunca incluiu. Mantenha a árvore de dependências compacta, auditável e resiliente.

---

## 📈 Atividades recentes

```text
Sprint atual:
  [■■■■■■■■■□] 90% - Migração do caminho de escrita WAL do vortex-db para io_uring assíncrono
  [■■■■■■□□□□] 60% - Implementação da transferência de snapshots de máquina de estados no raft-ring
  [■■■■■■■■■■] 100% - Lançamento do executor de perfil de latência wire-bench para Linux 6.8+
```

---

## 📬 Contato & Links

- **E-mail**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Fuso horário**: UTC+9 / Disponível para colaboração remota distribuída em projetos de código aberto
