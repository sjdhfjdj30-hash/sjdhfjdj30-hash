| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Hola, soy Marcus Vance 👋

Ingeniero de software de sistemas especializado en **redes de baja latencia**, **motores de almacenamiento embebidos** y **algoritmos de consenso distribuido**.

Diseño y construyo infraestructura determinista y eficiente en el uso de memoria, con énfasis en la simpatía mecánica (Mechanical Sympathy), protocolos de red sin asignaciones intermedias (zero-allocation) y semántica robusta de recuperación ante fallos. Creo firmemente que el software debe ser rápido, minimalista y observable por defecto.

---

## 🔭 Proyectos activos y código abierto

| Proyecto | Lenguaje | Arquitectura y propósito | Estado |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Motor de almacenamiento embebido LSM-tree de copia cero optimizado para escritura, con memtables concurrentes, compactación por niveles y WAL de E/S directa. | Motor central v0.8.2 |
| **raft-ring** | Go | Implementación minimalista del consenso Raft con capas de transporte intercambiables (QUIC / gRPC) y descubrimiento de membresía mediante protocolo Gossip (SWIK). | En desarrollo activo |
| **wire-bench** | C++20 | Suite de pruebas de rendimiento de sockets de precisión de microsegundos que evalúa latencias de cola TCP/UDP utilizando `io_uring` de Linux y puntos de traza eBPF. | Versión estable v1.2.0 |
| **kflow** | Go | Herramienta TUI nativa para terminal que monitorea en tiempo real el tráfico de particiones Kafka, eventos de rebalanceo y retraso de consumidores. | Código abierto |

---

## 🛠️ Pila técnica y herramientas

| Categoría | Tecnologías principales |
| :--- | :--- |
| **Lenguajes** | Rust, Go, C++20, C, Zig, Python (herramientas), Bash |
| **Almacenamiento y datos** | LSM-Trees, B-Trees, arquitectura interna de RocksDB, PostgreSQL, Redis, Apache Kafka |
| **Sistemas y bajo nivel** | Programación de sistemas Linux, `io_uring`, epoll, eBPF, optimizaciones SIMD, alineación de líneas de caché |
| **Concurrencia y consenso** | Raft, Paxos, buffers circulares sin bloqueo (lock-free ring buffers), colas MPMC |
| **Observabilidad y perfiles** | Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints, OpenTelemetry |
| **Entorno de trabajo** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Principios de ingeniería

- **Simpatía mecánica ante todo**: Comprender la jerarquía de memoria, los límites de las líneas de caché de la CPU y los predictores de saltos antes de intentar optimizar cualquier código.
- **Métricas antes que suposiciones**: "En Dios confiamos; todos los demás deben aportar microbenchmarks reproducibles y diagramas de llama (flamegraphs)."
- **Diseño tolerante a caídas (Crash-Only)**: Todo motor de almacenamiento debe ser capaz de recuperarse limpiamente tras un corte abrupto de energía o una señal SIGKILL en cualquier instrucción.
- **Dependencias mínimas**: La mejor dependencia es la que nunca se agregó. Mantener el árbol de dependencias compacto, auditable y resistente.

---

## 📈 Actividad reciente

```text
Sprint actual:
  [■■■■■■■■■□] 90% - Migración de la ruta de volcado WAL de vortex-db a io_uring asíncrono
  [■■■■■■□□□□] 60% - Implementación de la transferencia de instantáneas de máquina de estados en raft-ring
  [■■■■■■■■■■] 100% - Lanzamiento del ejecutor de perfiles wire-bench para Linux 6.8+
```

---

## 📬 Contacto y enlaces

- **Correo electrónico**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Zona horaria**: UTC+9 / Disponible para colaboración remota distribuida en proyectos de código abierto
