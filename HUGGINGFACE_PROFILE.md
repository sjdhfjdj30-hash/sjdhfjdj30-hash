# Marcus Vance (@fsafaw34r)

Senior Systems Software Engineer focusing on **high-throughput compute runtimes**, **zero-copy data serialization**, and **embedded vector storage engines**.

Primary GitHub Hub: [github.com/sjdhfjdj30-hash](https://github.com/sjdhfjdj30-hash)

---

## 🔬 Systems & Computational Infrastructure Focus

I focus on the intersection of **low-level systems software** and **numerical compute infrastructure**:

- **Zero-Copy Weight Streaming**: Direct `mmap` and `io_uring`-driven loaders for GGUF and SafeTensors formats to eliminate CPU memory copying during data loading.
- **Embedded Vector Indexes**: LSM-tree-backed HNSW vector storage designed for edge devices and memory-constrained environments.
- **Micro-Kernel Profiling**: Microsecond-precision benchmarking of numeric computation kernels across modern CPU SIMD extensions (AVX-512, NEON).
- **Mechanical Sympathy in Memory Access**: Designing paging and batching systems aligned with CPU/GPU memory channel bandwidth limits and cache hierarchies.

---

## 📦 Planned Tools, Benchmarks & Datasets

| Artifact | Category | Description | Primary Stack |
| :--- | :--- | :--- | :--- |
| **direct-gguf-streamer** | Space / Tool | Linux `io_uring` direct-I/O loader benchmarking multi-gigabyte weight streaming throughput. | Rust / C |
| **lsm-hnsw-bench** | Dataset | Comparative latency and recall benchmarks of LSM-tree vs Flat file vector index layouts. | JSON / Parquet |
| **quant-simd-kernels** | Space / Tool | Interactive comparative latency viewer for hand-crafted AVX-512 and ARM NEON numerical kernels. | Rust / WebAssembly |

---

## 🛠️ Core Tech Stack

| Domain | Stack |
| :--- | :--- |
| **Languages** | Rust, C++20, C, Python, Go |
| **Formats & Engines** | GGUF, SafeTensors, ONNX Runtime internals, SIMD Vectorization |
| **Low-Level I/O** | Linux `io_uring`, POSIX AIO, SIMD Intrinsics, Cache-line alignment |
| **Primary Code Repository** | [github.com/sjdhfjdj30-hash](https://github.com/sjdhfjdj30-hash) |

---

## 📬 Contact

- **Email**: `sjdhfjdj30@gmail.com`
- **GitHub**: [`@sjdhfjdj30-hash`](https://github.com/sjdhfjdj30-hash)
- **Hugging Face**: [`@fsafaw34r`](https://huggingface.co/fsafaw34r)
