# AI Infrastructure Engineering — Learning Roadmap

**66 Topics | 10 Phases | Beginner to Production**

**Certification Targets:** NVIDIA NCA-AIIO and NCP-AII

**Learning Sequence:** Computer Fundamentals → GPU & CUDA → AI Servers → Networking → Storage → Cluster Operations → Validation → Production

## Phase 01 — Computer & Hardware Foundations

*Goal: Understand the components and operating systems underlying AI infrastructure.*

- [ ] **Day 01:** What is a CPU? — Architecture, instructions, ISA, and CPU responsibilities.
- [ ] **Day 02:** CPU Cores, Threads, Clock Speed & Performance — SMT, utilization, vCPUs, and bottlenecks.
- [ ] **Day 03:** RAM, Cache & Memory Hierarchy — Latency, bandwidth, NUMA, and memory access.
- [ ] **Day 04:** What is a GPU? — GPU fundamentals, parallel processing, and applications.
- [ ] **Day 05:** CPU vs GPU — Architectural differences and heterogeneous computing.
- [ ] **Day 06:** Parallel Computing Fundamentals — Concurrency, SIMD, SIMT, and workload parallelism.
- [ ] **Day 07:** Linux & System Administration — Processes, permissions, services, logs, and resource inspection.
- [ ] **Day 08:** Computer & AI Server Architecture — CPU sockets, PCIe, NICs, storage, and device topology.

**Milestone:** Linux CPU and Memory Inspection Lab.

## Phase 02 — NVIDIA GPU & CUDA Fundamentals

*Goal: Understand GPU execution and the NVIDIA software/hardware environment.*

- [ ] **Day 09:** NVIDIA GPU Architecture — SMs, CUDA cores, Tensor Cores, and GPU generations.
- [ ] **Day 10:** What is CUDA? — Accelerated computing, host/device model, and kernels.
- [ ] **Day 11:** NVIDIA Drivers, CUDA Runtime & Toolkit — Installation concepts and compatibility.
- [ ] **Day 12:** CUDA Execution Model — Threads, blocks, grids, and kernel launches.
- [ ] **Day 13:** CUDA Memory Architecture — Global, shared, local, and constant memory.
- [ ] **Day 14:** GPU Performance Fundamentals — Utilization, bandwidth, occupancy, and bottlenecks.
- [ ] **Day 15:** GPU Monitoring & Troubleshooting — NVIDIA-SMI, DCGM, and error investigation.
- [ ] **Day 16:** PCIe, NVLink & NVSwitch — GPU interconnects and device communication.
- [ ] **Day 17:** GPU Partitioning & MIG — Resource allocation, isolation, and sharing.
- [ ] **Day 18:** GPU Infrastructure Validation — Basic CUDA execution, driver verification, and operational checks.

**Milestone:** NVIDIA GPU Validation Lab (requires compatible GPU access).

**Note:** Detailed CUDA C++ programming exercises will be maintained separately in `cuda-learning-lab`.

## Phase 03 — AI Server Architecture & Bring-up

*Goal: Understand NVIDIA GPU server installation and commissioning.*

- [ ] **Day 19:** NVIDIA DGX & HGX — Platforms, components, and server architecture.
- [ ] **Day 20:** AI Server Deployment Lifecycle — Planning, rack installation, and acceptance criteria.
- [ ] **Day 21:** BMC, OOB & TPM — Management interfaces, Redfish, and server security.
- [ ] **Day 22:** BIOS, UEFI & Firmware — Firmware inventory, upgrades, HGX components, and compatibility.
- [ ] **Day 23:** Physical GPU Installation — Hardware installation, component discovery, and validation.
- [ ] **Day 24:** Server Bring-up & Validation — Hardware health, power-on tests, and readiness checks.

**Milestone:** GPU Server Deployment and Validation Runbook.

## Phase 04 — AI Networking & NVIDIA Fabrics

*Goal: Understand high-performance AI networking and physical fabric validation.*

- [ ] **Day 25:** Networking Fundamentals — TCP/IP, routing, switching, Ethernet, VLANs, and MTU.
- [ ] **Day 26:** AI Factory Network Architecture — Leaf-spine topology and management/compute/storage fabrics.
- [ ] **Day 27:** RDMA, RoCE & InfiniBand — Remote memory access and high-speed communication.
- [ ] **Day 28:** NVIDIA Networking — ConnectX, Spectrum, InfiniBand switches, and BlueField.
- [ ] **Day 29:** NVIDIA BlueField & DOCA — DPU architecture, offloading, configuration, and management.
- [ ] **Day 30:** Cabling & Network Validation — DAC, AOC, optical transceivers, firmware, and signal quality.

**Milestone:** AI Cluster Networking and Cabling Validation Guide.

## Phase 05 — AI Storage, Power & Data Centers

*Goal: Understand supporting infrastructure and physical operational constraints.*

- [ ] **Day 31:** AI Storage Fundamentals — SSD, NVMe, NAS, block, file, and object storage.
- [ ] **Day 32:** High-Performance & Distributed Storage — Parallel filesystems and data access.
- [ ] **Day 33:** Storage Configuration & Validation — Mounts, IOPS, latency, throughput, and benchmarking.
- [ ] **Day 34:** AI Data Center Power — PSU, PDU, redundancy, and power budgets.
- [ ] **Day 35:** Cooling & Thermal Management — Air/liquid cooling, temperatures, and thermal validation.
- [ ] **Day 36:** AI Factory Infrastructure Planning — Racks, capacity, physical layout, and readiness.

**Milestone:** AI Data Center Infrastructure Readiness Checklist.

## Phase 06 — Linux, NVIDIA Drivers & Containers

*Goal: Configure the software environment required for AI workloads.*

- [ ] **Day 37:** Linux Server Installation & Configuration — Services, networking, SSH, and system management.
- [ ] **Day 38:** NVIDIA Drivers & CUDA Compatibility — Drivers, kernel modules, lifecycle, and validation.
- [ ] **Day 39:** NVIDIA DOCA Drivers — Driver management, dependencies, and upgrade considerations.
- [ ] **Day 40:** Docker Fundamentals — Images, containers, volumes, networks, and resource limits.
- [ ] **Day 41:** NVIDIA Container Toolkit — GPU-enabled containers and runtime verification.
- [ ] **Day 42:** NVIDIA NGC CLI — Installation, catalogs, container images, and authentication.

**Milestone:** Linux and NVIDIA GPU Container Deployment Lab.

## Phase 07 — AI Cluster Management

*Goal: Understand provisioning, scheduling, and operating GPU clusters.*

- [ ] **Day 43:** AI Cluster Architecture — Management nodes, compute nodes, networks, and HA.
- [ ] **Day 44:** NVIDIA Base Command Manager — Installation, provisioning, and configuration categories.
- [ ] **Day 45:** BCM High Availability — Cluster interfaces, redundancy, and failover validation.
- [ ] **Day 46:** Slurm Workload Scheduler — Partitions, jobs, queues, and resource scheduling.
- [ ] **Day 47:** Enroot & Pyxis — Containerized HPC jobs and Slurm integration.
- [ ] **Day 48:** Kubernetes & NVIDIA GPU Operator — Scheduling, device plugins, and GPU management.

**Milestone:** Cluster Management and Workload Scheduling Lab.

## Phase 08 — GPU, Node & Fabric Testing

*Goal: Learn infrastructure qualification and hardware verification.*

- [ ] **Day 49:** Infrastructure Testing Methodology — Acceptance tests, baselines, and pass/fail criteria.
- [ ] **Day 50:** Single-Node Stress Testing — CPU, memory, GPU stability, and health checks.
- [ ] **Day 51:** HPL Benchmarking — High-Performance Linpack and compute validation.
- [ ] **Day 52:** NCCL Testing — Collective communication, NVLink, NVSwitch, and bandwidth.
- [ ] **Day 53:** Network Fabric Verification — Cable diagnostics, switch firmware, errors, and transceivers.
- [ ] **Day 54:** NVIDIA ClusterKit — Cluster-wide node assessment and fabric testing.

**Milestone:** AI Cluster Qualification and Benchmark Report.

## Phase 09 — Burn-in & Performance Validation

*Goal: Validate stability and workload readiness under sustained load.*

- [ ] **Day 55:** Burn-in Testing Fundamentals — Sustained stress testing and failure criteria.
- [ ] **Day 56:** NCCL Burn-in — Multi-GPU communication and fabric stability.
- [ ] **Day 57:** HPL Burn-in — Compute performance and sustained hardware health.
- [ ] **Day 58:** NVIDIA NeMo Burn-in — AI workload testing and operational stability.
- [ ] **Day 59:** Storage Performance Testing — Throughput, latency, IOPS, and bottlenecks.
- [ ] **Day 60:** GPU Observability — DCGM, Prometheus, Grafana, logs, and alerting.

**Milestone:** Infrastructure Performance and Burn-in Report.

## Phase 10 — Troubleshooting & Production Operations

*Goal: Troubleshoot hardware, optimize performance, and prepare production handover.*

- [ ] **Day 61:** GPU, NIC & Hardware Faults — Diagnostics, fault isolation, and error analysis.
- [ ] **Day 62:** GPU, PSU & Component Replacement — Maintenance procedures and post-repair validation.
- [ ] **Day 63:** Network & Storage Troubleshooting — Fabric failures, bandwidth, and storage bottlenecks.
- [ ] **Day 64:** Intel & AMD Server Optimization — NUMA, affinity, BIOS tuning, and performance.
- [ ] **Day 65:** Production Readiness & Operations — Reliability, change control, rollback, and handover.
- [ ] **Day 66:** Final AI Infrastructure Capstone — Design, provision, validate, troubleshoot, and document an AI cluster.

**Milestone:** End-to-End AI Infrastructure Engineering Portfolio Project.

---

## NVIDIA Certification Alignment

| NCP-AII Domain | Exam Weight | Main Phases |
|---|---|---|
| System & Server Bring-up | 31% | 03, 04, 05 |
| Physical Layer Management | 5% | 02, 04 |
| Control Plane Installation | 19% | 06, 07 |
| Cluster Test & Verification | 33% | 08, 09 |
| Troubleshoot & Optimize | 12% | 09, 10 |

The roadmap also covers foundational NCA-AIIO knowledge and practical engineering skills beyond the professional exam.

**Official Reference:** [NVIDIA NCP-AII Exam](https://www.nvidia.com/en-us/learn/certification/ai-infrastructure-professional/)

