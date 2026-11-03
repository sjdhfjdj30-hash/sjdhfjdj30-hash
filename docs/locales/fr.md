| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Bonjour, je suis Marcus Vance 👋

Ingénieur logiciel systèmes spécialisé dans les **réseaux à très faible latence**, les **moteurs de stockage embarqués** et les **algorithmes de consensus distribué**.

Je conçois et développe des infrastructures déterministes et économes en mémoire, en mettant l'accent sur la sympathie mécanique (Mechanical Sympathy), les protocoles réseau sans allocation intermédiaire (zero-allocation) et la résilience stricte face aux pannes. Je suis convaincu qu'un logiciel doit être rapide, simple et intrinsèquement observable.

---

## 🔭 Projets en cours et initiatives Open Source

| Projet | Langage | Architecture et objectifs | Statut |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Moteur de stockage embarqué LSM-tree à copie zéro, optimisé pour l'écriture avec memtables concurrentes, compactage étagé et WAL à E/S directes. | Moteur principal v0.8.2 |
| **raft-ring** | Go | Implémentation minimaliste de l'algorithme de consensus Raft avec couches de transport modulaires (QUIC / gRPC) et découverte de membres par protocole Gossip (SWIK). | En développement actif |
| **wire-bench** | C++20 | Suite de benchmarks de sockets réseau avec précision à la microseconde, analysant les latences extrêmes TCP/UDP via `io_uring` et les tracepoints eBPF. | Version stable v1.2.0 |
| **kflow** | Go | Outil de monitoring en interface texte (TUI) pour suivre en temps réel le trafic des partitions Kafka, les rééquilibrages et le décalage des consommateurs. | Open Source |

---

## 🛠️ Stack technique et boîte à outils

| Catégorie | Technologies et outils de prédilection |
| :--- | :--- |
| **Langages** | Rust, Go, C++20, C, Zig, Python (outillage), Bash |
| **Stockage & Données** | LSM-Trees, B-Trees, architecture interne de RocksDB, PostgreSQL, Redis, Apache Kafka |
| **Systèmes & Bas niveau** | Programmation système Linux, `io_uring`, epoll, eBPF, vectorisation SIMD, alignement sur lignes de cache |
| **Concurrence & Consensus** | Raft, Paxos, tampons circulaires sans verrou (lock-free ring buffers), files MPMC |
| **Observabilité & Profilage** | Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints, OpenTelemetry |
| **Environnement de travail** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Principes d'ingénierie

- **Sympathie mécanique avant tout** : Maîtriser la hiérarchie de la mémoire, les limites des lignes de cache du processeur et les mécanismes de prédiction de branchement avant d'optimiser le moindre code.
- **Les benchmarks plutôt que les hypothèses** : « En Dieu nous croyons ; tous les autres doivent apporter des microbenchmarks reproductibles et des flamegraphs. »
- **Conception orientée crash (Crash-Only)** : Tout moteur de stockage doit être capable de récupérer intégralement et sans corruption après une coupure de courant soudaine ou un SIGKILL.
- **Dépendances minimales** : La meilleure dépendance est celle que vous n'avez jamais ajoutée. Garder l'arbre des dépendances concis, auditable et résilient.

---

## 📈 Activités récentes

```text
Sprint en cours :
  [■■■■■■■■■□] 90% - Migration du chemin d'écriture WAL de vortex-db vers io_uring asynchrone
  [■■■■■■□□□□] 60% - Implémentation du transfert d'instantanés de la machine à états dans raft-ring
  [■■■■■■■■■■] 100% - Publication de wire-bench pour Linux 6.8+
```

---

## 📬 Contact & Liens

- **E-mail** : `sjdhfjdj30@gmail.com`
- **GitHub** : [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Fuseau horaire** : UTC+9 / Ouvert aux collaborations Open Source distribuées dans le monde entier
