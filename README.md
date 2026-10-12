# Awesome Unsigned [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated catalog of autonomous agent orchestrators, pooled harnesses, bare-metal infrastructure, and machine sympathy research across [unsigned.gg](https://unsigned.gg) and the open systems community.

The infrastructure provides open, forkable compute, storage, and scheduling at commodity utility rates.

---

## Mission & Public Domain Charter

> *"A better future through mutual cooperation between man and machine."*

The **unsigned** organization exists to test agent swarm control, governance, and security in production environments.
While conducting these tests, the organization publishes foundational research on machine sympathy, systems security, and mathematical- and engineering-driven development:

* **Swarm Control, Governance & Security:** Testing autonomous agent fleets, capability confinement, Landlock LSM containment, and cryptographic attestation.
* **Machine Sympathy:** Hardware-sympathetic systems engineering, zero-allocation domain crates, `pidfd` process management, and deterministic instruction-count profiling.
* **Mathematical & Engineering-Driven Development:** Operational semantics, model checking, and formal verification over empirical guesswork.
* **Permanent Public Domain:** All work, codebases, specifications, and research findings in this organization remain permanently in the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

### Community Constitution & Standards
* [Commitments to Privacy, Freedom, and Dignity](https://github.com/unsigned-gg/.github/blob/main/PRIVACY_FREEDOM_DIGNITY.md) — Mutual cooperation between man and machine, local-first computing, zero telemetry.
* [Guiding Principles, Mottos & Northstars](https://github.com/unsigned-gg/.github/blob/main/GUIDING_PRINCIPLES.md) — Machine sympathy, soundness over speed, and strategic objectives.
* [Community Standards & Code of Conduct](https://github.com/unsigned-gg/.github/blob/main/COMMUNITY_STANDARDS.md) — Intellectual honesty, blameless inquiry, and mutual respect.
* [Brand Voice & Style Guide](https://github.com/unsigned-gg/.github/blob/main/BRAND_VOICE.md) — ASD-STE100 precision and the Cat B hacker register.

---

## Contents

- [Mission & Public Domain Charter](#mission--public-domain-charter)
- [The Orchestrator & Autonomous Workforces](#the-orchestrator--autonomous-workforces)
- [Agent Substrates & Runtimes](#agent-substrates--runtimes)
- [Process Supervision & Systems Core](#process-supervision--systems-core)
- [Multi-Agent Observability & Telemetry](#multi-agent-observability--telemetry)
- [Deterministic Dispatch & Scheduling](#deterministic-dispatch--scheduling)
- [Sandboxing & Execution Containment](#sandboxing--execution-containment)
- [Bare-Metal & Infrastructure](#bare-metal--infrastructure)
- [Contributing](#contributing)
- [License](#license)

---

## The Orchestrator & Autonomous Workforces

- [k8](https://github.com/unsigned-gg/k8) — Kubernetes agent orchestrator, workload controller, and native CLI tooling for autonomous agent fleets.
- [gs](https://github.com/unsigned-gg/gs) — Godseat control surface: operator cluster surface governing perception before action and policy gate tiers.
- [soma](https://github.com/unsigned-gg/soma) — The agentic OS: governed autonomy over a persistent agent workforce (`soma-os`, terrarium federated node).
- [dc](https://github.com/unsigned-gg/dc) — Dark compute & mission control: live agent orchestration surface, AgentHub Durable Object, live fleet monitoring.
- [dgr](https://github.com/unsigned-gg/dgr) — Real-time terminal graph renderer: renders autonomous swarm execution DAGs with animated state transitions.

---

## Agent Substrates & Runtimes

- [uas](https://github.com/unsigned-gg/uas) — Unsigned Agent Substrate: Rust-native pooled harness runtime with strict zero-I/O domain layering.

---

## Process Supervision & Systems Core

- [kd](https://github.com/unsigned-gg/kd) — Pure-Rust Linux process supervisor using native `pidfd` handles and epoll loops for zombie-free supervision.
- [od](https://github.com/unsigned-gg/od) — Terminal multiplexing hook with high TTY throughput for headless agent workloads.

---

## Multi-Agent Observability & Telemetry

- [access-tui](https://github.com/unsigned-gg/access-tui) — Live view of connected estate systems and agent channels.
- [toolmon](https://github.com/unsigned-gg/toolmon) — Fleet monitoring of in-house agent tools, versions, and drift across machines.

---

## Deterministic Dispatch & Scheduling

- [ep](https://github.com/unsigned-gg/ep) — Escapement scheduler: metered, deterministic dispatch engine for autonomous agent swarms (`ep-serve` orchestrator daemon).
- [wak](https://github.com/unsigned-gg/wak) — Accept-and-hold TCP wake proxy and idle reaper for scale-to-zero workloads.

---

## Sandboxing & Execution Containment

- [sbx](https://github.com/unsigned-gg/sbx) — AI-containment layer for agent execution: OS syscall jail with reversible run-custody records in Rust.
- [reach](https://github.com/unsigned-gg/reach) — AI-drivable containerized desktop sandbox.
- [overflow](https://github.com/unsigned-gg/overflow) — GPU-accelerated, agent-aware terminal emulator in Rust (wgpu, ConPTY).

---

## Bare-Metal & Infrastructure

- [unsigned-paas](https://github.com/unsigned-gg/unsigned-paas) — Kubernetes-native AI/ML PaaS: bare-metal Talos, Helm, ArgoCD, and GPU scheduling.
- [metal-foundry](https://github.com/unsigned-gg/metal-foundry) — Talos Image Factory schematics, PXE bring-up, and bare-metal upgrade drills.
- [cadastre](https://github.com/unsigned-gg/cadastre) — Alchemy IaC control plane for cloud and edge infrastructure.

---

## Contributing

Contributions are welcome. Open an issue or pull request. Follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).

---

## License

All software, documentation, and research in this repository are dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
