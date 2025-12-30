---
title: "ORION"
date: 2025-12-30
summary: "A next-generation CFD solver designed for multi-block structured grids on CPU/GPU heterogeneous HPC systems."

# 建议：封面图可以使用 ORION 架构图或大规模并行计算的渲染图
featureImage: "img/LOGO-ORION.png" 

tags: ["C++", "CUDA", "MPI", "HPC", "Heterogeneous Computing"]
---

[cite_start]**ORION** is a high-performance, extensible CFD solver framework specifically engineered for large-scale **multi-block structured grids** on modern **heterogeneous HPC systems**.

### 🚀 Core Capabilities

[cite_start]The framework is built to achieve extreme computational efficiency while maintaining long-term extensibility across various hardware architectures.

* [cite_start]**Multi-block Structured Grid**: Supports arbitrary block connectivity and efficient halo exchange via MPI.
* [cite_start]**Heterogeneous Computing**: Architecture-neutral design with native backends for **CPU, CUDA, and HIP**, with upcoming support for DCU.
* [cite_start]**High-Performance Parallelism**: Utilizes a CUDA-aware MPI model, overlapping computation and communication to maximize throughput.
* [cite_start]**Scalable Physics**: Includes modular support for compressible Navier–Stokes equations, with RANS models and implicit time-marching in development.



### 🏗️ Software Architecture

[cite_start]ORION adopts a strict **Separation of Concerns** philosophy. [cite_start]The architecture is divided into independent, testable modules:

| Module | Responsibility |
| :--- | :--- |
| **core** | [cite_start]Parallel runtime, memory management, and utilities  |
| **mesh & field** | [cite_start]Structured grid management and SoA (Structure of Arrays) data layout  |
| **numerics** | [cite_start]High-order reconstruction, flux schemes, and operators  |
| **comm** | [cite_start]Asynchronous halo exchange and MPI communication  |
| **io** | [cite_start]Solver-I/O decoupled design with ParaView-compatible VTS/VTM output  |

### 💡 Parallel Execution Model

[cite_start]ORION organizes computation at the **block level**, which serves as the fundamental unit for execution and communication. [cite_start]A typical timestep involves:
1.  [cite_start]**Interior Computation**: Processing the core of the block.
2.  [cite_start]**Asynchronous Exchange**: Overlapping halo data transfer with computation.
3.  [cite_start]**Boundary Computation**: Completing calculations at the interfaces.
4.  [cite_start]**Update**: Final time integration step.

### 🔗 Project Status & Access

[cite_start]ORION is currently under active research and development. [cite_start]Key milestones include the deployment of the multi-backend abstraction layer and implicit solvers.

{{< button href="https://github.com/zhanghong24/ORION" target="_blank" >}}
  Explore on GitHub
{{< /button >}}