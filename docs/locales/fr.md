| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# Bonjour, je suis Marcus Vance 👋

Ingénieur Logiciel Systèmes Senior spécialisé dans les **réseaux à très faible latence**, les **moteurs de stockage embarqués** et les **protocoles de consensus distribué**.

Je conçois des infrastructures déterministes et hautement efficientes en mémoire, avec une exigence absolue de sympathie mécanique (Mechanical Sympathy), de protocoles réseau à zéro allocation et de sémantique robuste de récupération après crash. Je crois que le logiciel doit être fondamentalement rapide, transparent et résilient par premiers principes.

---

## 🔭 Projets d'Ingénierie Principaux

| Projet | Langage | Architecture & Objectifs | Statut |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Moteur de stockage embarqué LSM-tree optimisé pour l'écriture et le zero-copy, intégrant des memtables concurrentes, un compactage par paliers et un WAL à E/S directes. | Moteur Core v0.8.2 |
| **raft-ring** | Go | Implémentation performante du consensus Raft avec couches de transport interchangeables (QUIC / gRPC) et découverte de membres SWIK gossip. | Développement Actif |
| **wire-bench** | C++20 | Suite de benchmarks de sockets avec précision à la microseconde évaluant les latences extrêmes TCP/UDP via Linux `io_uring` et points de trace eBPF. | Version Stable v1.2.0 |
| **kflow** | Go | Outil de supervision TUI natif en terminal pour l'analyse en temps réel du trafic de partitions Kafka, des rééquilibrages et du lag consommateur. | Open Source |

---

## 🛠️ Stack Technique & Boîte à Outils

| Catégorie | Technologies Clés |
| :--- | :--- |
| **Langages** | Rust, Go, C++20, C, Zig, Python (Outillage interne), Bash |
| **Stockage & Moteurs** | LSM-Trees, B-Trees, Internals RocksDB, PostgreSQL, Redis, Apache Kafka |
| **Systèmes & Bas Niveau** | Programmation Système Linux, `io_uring`, epoll, eBPF, Optimisations SIMD, Alignement de ligne de cache |
| **Concurrence & Consensus**| Raft, Paxos, Buffers circulaires lock-free, Files MPMC |
| **Observabilité & Profilage**| Linux `perf`, Flamegraphs, Valgrind, LLDB, Points de trace eBPF |
| **Environnement** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Principes d'Ingénierie

- **Sympathie Mécanique d'Abord**: Comprendre la hiérarchie mémoire physique, l'alignement des lignes de cache et les prédicteurs de branchement avant toute optimisation.
- **Les Mesures Avant les Suppositions**: « En Dieu nous croyons ; tous les autres doivent fournir des micro-benchmarks reproductibles et des flamegraphs. »
- **Conception Orientée Crash (Crash-Only)**: Tout système de stockage doit être capable de récupérer proprement après une coupure d'alimentation brutale ou un SIGKILL sur n'importe quelle instruction.
- **Dépendances Minimales**: La meilleure dépendance est celle que vous n'avez jamais ajoutée. Garder le graphe de dépendances compact, vérifiable et robuste.

---

## 📈 Focus de Développement Actuel

```text
Sprint Actuel :
  [■■■■■■■■■□] 90% - Migration du chemin de vidage WAL de vortex-db vers io_uring asynchrone
  [■■■■■■□□□□] 60% - Implémentation des transferts de machine à états par snapshot dans raft-ring
  [■■■■■■■■■■] 100% - Publication du profileur de latence wire-bench pour Linux 6.8+
```

---

## 📬 Contact & Liens

- **E-mail**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Fuseau Horaire**: UTC+9 / Disponible pour la collaboration sur des systèmes distribués dans le monde entier
