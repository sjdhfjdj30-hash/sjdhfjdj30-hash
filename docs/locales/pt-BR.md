| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# Olá, sou Marcus Vance 👋

Engenheiro de Software de Sistemas Sênior especializado em **redes de ultra-baixa latência**, **motores de armazenamento embarcados** e **protocolos de consenso distribuído**.

Desenvolvo infraestrutura determinística e com alta eficiência de memória, priorizando a empatia mecânica com o hardware (Mechanical Sympathy), protocolos de rede com alocação zero de memória e semânticas confiáveis de recuperação de falhas. Acredito que o software deve ser veloz, transparente e resiliente por primeiros princípios.

---

## 🔭 Principais Projetos de Engenharia

| Projeto | Linguagem | Arquitetura e Foco | Status |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Motor de armazenamento embarcado LSM-tree otimizado para escrita e sem cópias (zero-copy), com memtables concorrentes, compactação em camadas e WAL de E/S direta. | Motor Principal v0.8.2 |
| **raft-ring** | Go | Implementação de alto desempenho do consenso Raft com camadas de transporte intercambiáveis (QUIC / gRPC) e descoberta de nós via gossip. | Desenvolvimento Ativo |
| **wire-bench** | C++20 | Conjunto de benchmarks de sockets com precisão de microssegundos para avaliar latências extremas TCP/UDP via Linux `io_uring` e eBPF tracepoints. | Versão Estável v1.2.0 |
| **kflow** | Go | Ferramenta TUI nativa de terminal para monitorar em tempo real o tráfego de partições do Kafka, eventos de rebalanceamento e lag de consumidores. | Código Aberto |

---

## 🛠️ Stack Técnico e Ferramentas

| Categoria | Tecnologias Principais |
| :--- | :--- |
| **Linguagens** | Rust, Go, C++20, C, Zig, Python (Ferramentas internas), Bash |
| **Armazenamento e Motores** | LSM-Trees, B-Trees, Estrutura interna do RocksDB, PostgreSQL, Redis, Apache Kafka |
| **Sistemas e Baixo Nível** | Programação de Sistemas Linux, `io_uring`, epoll, eBPF, Otimizações SIMD, Alinhamento de linhas de cache |
| **Concorrência e Consenso**| Raft, Paxos, Buffers circulares lock-free, Filas MPMC |
| **Observabilidade e Profiling**| Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints |
| **Ambiente de Desenvolvimento**| Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Filosofia de Engenharia

- **Empatia Mecânica Primeiro (Mechanical Sympathy)**: Compreender a hierarquia de memória física, limites de linha de cache e previsores de desvio antes de otimizar código.
- **Métricas Acima de Suposições**: "Em Deus nós confiamos; todos os outros devem apresentar micro-benchmarks reprodutíveis e flamegraphs."
- **Design Voltado a Falhas (Crash-Only Design)**: Qualquer sistema de armazenamento deve ser capaz de recuperar a integridade de dados perfeitamente após corte súbito de energia ou sinal SIGKILL em qualquer instrução.
- **Dependências Mínimas**: A melhor dependência é aquela que você nunca adicionou. Manter a árvore de dependências enxuta, auditável e confiável.

---

## 📈 Foco de Desenvolvimento Atual

```text
Sprint Atual:
  [■■■■■■■■■□] 90% - Migrando o fluxo de gravação de WAL do vortex-db para io_uring assíncrono
  [■■■■■■□□□□] 60% - Implementando transferência de máquina de estados por snapshot no raft-ring
  [■■■■■■■■■■] 100% - Lançamento do perfilador de latência wire-bench para Linux 6.8+
```

---

## 📬 Contato e Links

- **E-mail**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Fuso Horário**: UTC+9 / Disponível para colaboração remota em sistemas distribuídos de código aberto
