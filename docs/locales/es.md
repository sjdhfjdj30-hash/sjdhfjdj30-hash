| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [SA العربية](./ar.md) | [IN हिन्दी](./hi.md) |

---

# Hola, soy Marcus Vance 👋

Ingeniero de Software de Sistemas Senior especializado en **redes de baja latencia**, **motores de almacenamiento embebidos** y **protocolos de consenso distribuido**.

Diseño infraestructura determinista y de memoria eficiente con un enfoque inquebrantable en la simpatía mecánica (Mechanical Sympathy), protocolos de red de cero asignación y semánticas sólidas de recuperación ante fallos. Creo firmemente que el software debe ser rápido, transparente y resiliente por primeros principios.

---

## 🔭 Proyectos Principales de Ingeniería

| Proyecto | Lenguaje | Arquitectura y Enfoque | Estado |
| :--- | :--- | :--- | :--- |
| **vortex-db** | Rust | Motor de almacenamiento embebido LSM-tree optimizado para escritura y sin copias (zero-copy), con memtables concurrentes, compactación por niveles y WAL de E/S directa. | Motor Principal v0.8.2 |
| **raft-ring** | Go | Implementación de alto rendimiento del consenso Raft con capas de transporte intercambiables (QUIC / gRPC) y descubrimiento de membresía SWIK. | Desarrollo Activo |
| **wire-bench** | C++20 | Suite de benchmarking de sockets de precisión de microsegundos que evalúa latencias de cola TCP/UDP usando `io_uring` y puntos de traza eBPF en Linux. | Versión Estable v1.2.0 |
| **kflow** | Go | Herramienta TUI nativa de terminal para monitorizar en tiempo real el tráfico de particiones Kafka, rebalanceos y retraso de consumidores. | Código Abierto |

---

## 🛠️ Stack Técnico y Herramientas

| Categoría | Tecnologías Principales |
| :--- | :--- |
| **Lenguajes** | Rust, Go, C++20, C, Zig, Python (Herramientas internas), Bash |
| **Almacenamiento y Motores** | LSM-Trees, B-Trees, RocksDB internals, PostgreSQL, Redis, Apache Kafka |
| **Sistemas y Bajo Nivel** | Programación de Sistemas Linux, `io_uring`, epoll, eBPF, Optimizaciones SIMD, Alineación de líneas de caché |
| **Concurrencia y Consenso**| Raft, Paxos, Buffers circulares lock-free, Colas MPMC |
| **Observabilidad y Perfilado**| Linux `perf`, Flamegraphs, Valgrind, LLDB, eBPF Tracepoints |
| **Entorno de Trabajo** | Neovim, Tmux, Alacritty, Docker, Git, Make/CMake, Linux Kernel 6.x |

---

## 📐 Principios de Ingeniería

- **Simpatía Mecánica Primero**: Comprender la jerarquía de memoria física, los límites de línea de caché y los predictores de saltos antes de optimizar código.
- **Métricas sobre Suposiciones**: "En Dios confiamos; todos los demás deben aportar microbenchmarks reproducibles y diagramas de llama (flamegraphs)."
- **Diseño Orientado al Fallo (Crash-Only)**: Todo sistema de almacenamiento debe ser capaz de recuperarse limpiamente tras una pérdida de energía abrupta o un SIGKILL en cualquier instrucción arbitraria.
- **Dependencias Mínimas**: La mejor dependencia es la que nunca agregaste. Mantener el árbol de dependencias reducido, auditable y resistente.

---

## 📈 Foco Actual de Desarrollo

```text
Sprint Actual:
  [■■■■■■■■■□] 90% - Portando la ruta de descarga WAL de vortex-db a io_uring asíncrono
  [■■■■■■□□□□] 60% - Implementando transferencias de máquina de estado con snapshots en raft-ring
  [■■■■■■■■■■] 100% - Publicando el perfilador de latencia wire-bench para Linux 6.8+
```

---

## 📬 Contacto y Enlaces

- **Correo**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Zona Horaria**: UTC+9 / Disponible para colaboración remota en sistemas distribuidos
