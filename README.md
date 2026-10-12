# Awesome Unsigned [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated catalog of autonomous agent orchestrators, pooled harnesses, bare-metal infrastructure, and machine sympathy research across [unsigned.gg](https://unsigned.gg) and the open systems community.

The engine: open, forkable compute, storage, and scheduling priced like plumbing.

---

## Mission & Public Domain Charter

> *"A better future through mutual cooperation between man and machine."*

The **unsigned** organization exists to test agent swarm control, governance, and security in production environments.
While running these tests, the organization lands foundational research on machine sympathy, systems security, and mathematical- and engineering-driven development:

* **Swarm Control, Governance & Security:** Testing autonomous agent fleets, capability confinement, Landlock LSM containment, and cryptographic attestation.
* **Machine Sympathy:** Hardware-sympathetic systems engineering, zero-allocation domain crates, `pidfd` process management, and deterministic instruction-count profiling.
* **Mathematical & Engineering-Driven Development:** Operational semantics, model checking, and formal verification over empirical guesswork.
* **Permanent Public Domain:** All work, codebases, specifications, and research findings in this organization remain permanently in the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

### Community Constitution & Standards
* [Commitments to Privacy, Freedom, and Dignity](https://github.com/unsigned-gg/.github/blob/main/PRIVACY_FREEDOM_DIGNITY.md) — Mutual cooperation between man and machine, local-first computing, zero telemetry.
* [Guiding Principles, Mottos & Northstars](https://github.com/unsigned-gg/.github/blob/main/GUIDING_PRINCIPLES.md) — Machine sympathy, soundness over speed, and the Northstars.
* [Community Standards & Code of Conduct](https://github.com/unsigned-gg/.github/blob/main/COMMUNITY_STANDARDS.md) — Intellectual honesty, blameless inquiry, and mutual respect.
* [Brand Voice & Style Guide](https://github.com/unsigned-gg/.github/blob/main/BRAND_VOICE.md) — ASD-STE100 precision and the Cat B hacker register.

---

## The Namespace Strategy

### Tactical 2-Letter Targets (8.1% Available)
Out of 676 two-letter permutations on crates.io, 55 remain open. Unsigned prioritizes six tactical targets:
* [**kd**](https://github.com/unsigned-gg/kd) — Pure-Rust Linux process supervisor using native `pidfd` handles and epoll loops (zero zombies).
* [**ep**](https://github.com/unsigned-gg/ep) — Escapement scheduler: metered, deterministic dispatch engine and event reactor.
* [**dc**](https://github.com/unsigned-gg/dc) — Dark compute runner: headless compute executor, dark factory scheduler, and desired configuration reconciler.
* [**gs**](https://github.com/unsigned-gg/gs) — Godseat control surface: operator cluster surface governing perception before action and policy gate tiers.
* [**kl**](https://github.com/unsigned-gg/kl) — Kernel link eBPF: Linux Landlock LSM file rules, seccomp BPF syscall filters, and eBPF probes.
* [**ls**](https://github.com/unsigned-gg/ls) — LeanSpec parser: formal Lean specification parser, structural AST validator, and CAS listing engine.

### Core 3-Letter Systems Matrix
* [**dgr**](https://github.com/unsigned-gg/dgr) — DAG engine: Directed Acyclic Graph execution engine & Ratatui visualizer (dual binaries `dgr`/`dagr`).
* [**sbx**](https://github.com/unsigned-gg/sbx) — Sandbox container framework: OS syscall jail with Landlock containment (live `v0.1.0` on crates.io).
* **nrn** — Neuron reflex head: calibrated reflex classifier and system-one decision network.
* [**wak**](https://github.com/unsigned-gg/waker) — Signal mesh: accept-and-hold TCP wake proxy and idle container reaper (`waker`).
* [**ovf**](https://github.com/unsigned-gg/overflow) — Ring buffer: GPU-accelerated terminal emulator and overflow PTY buffer (`overflow`).
* [**pgt**](https://github.com/unsigned-gg/pgt) — Epistemic swapper: Pretty Good Types memory engine for observation decay and knowledge folding.
* **sma** — Microkernel domain: Soma microkernel domain providing federated capability tokens and agentic OS primitives.

### The Anti-Squatting Rule
* **24-Hour Deletion Lock:** Any crate deletion on crates.io triggers an exact 24-hour registry lock on that name.
* **Substantive Code Mandate:** Unsigned prohibits empty placeholder crates. Every reservation must publish working, compilation-verified code immediately.

---

## Contents

- [Mission & Public Domain Charter](#mission--public-domain-charter)
- [The Namespace Strategy](#the-namespace-strategy)
- [The Orchestrator & Autonomous Workforces](#the-orchestrator--autonomous-workforces)
- [Agent Substrates & Runtimes](#agent-substrates--runtimes)
- [Process Supervision & Systems Core](#process-supervision--systems-core)
- [Session Multiplexing & Multi-Agent Observability](#session-multiplexing--multi-agent-observability)
- [Deterministic Dispatch & Scheduling](#deterministic-dispatch--scheduling)
- [Sandboxing & Execution Containment](#sandboxing--execution-containment)
- [Bare-Metal & Infrastructure](#bare-metal--infrastructure)
- [Contributing](#contributing)
- [License](#license)

---

## The Orchestrator & Autonomous Workforces

- [k8](https://github.com/unsigned-gg/k8) — Kubernetes agent orchestrator, workload controller, and native CLI tooling for autonomous agent fleets.
- [ep](https://github.com/unsigned-gg/ep) — Escapement scheduler: metered, deterministic dispatch engine for autonomous agent swarms (`ep-serve` orchestrator daemon).
- [soma](https://github.com/unsigned-gg/soma) — The agentic OS: governed autonomy over a persistent agent workforce (`soma-os`, terrarium federated node).
- [dc](https://github.com/unsigned-gg/dc) — Dark compute & mission control: live agent orchestration surface, AgentHub Durable Object, live fleet monitoring.
- [dgr](https://github.com/unsigned-gg/dgr) — Real-time terminal graph renderer: renders autonomous swarm execution DAGs with animated state transitions.
- [herdr-dagr](https://github.com/unsigned-gg/herdr-dagr) — Agent swarm as a live DAG: orchestration graph with attempts, review gates, and evidence in a split pane.

---

## Agent Substrates & Runtimes

- [uas](https://github.com/unsigned-gg/uas) — Unsigned Agent Substrate: Rust-native pooled harness runtime with strict zero-I/O domain layering.
- [substrate](https://github.com/unsigned-gg/substrate) — Execution runtime primitives for persistent agent processes.
- [ax](https://github.com/unsigned-gg/ax) — Open agentic orchestration runtime.

---

## Process Supervision & Systems Core

- [kd](https://github.com/unsigned-gg/kd) — Pure-Rust Linux process supervisor using native `pidfd` handles and epoll loops for zombie-free supervision.
- [od](https://github.com/unsigned-gg/od) — High-throughput TTY overdrive terminal multiplexing hook for headless agent workloads.

---

## Session Multiplexing & Multi-Agent Observability

- [herdr](https://github.com/unsigned-gg/herdr) — The runtime your coding agents live on: socket API, multi-agent pane orchestration, and session state without tmux.
- [herdr-norn](https://github.com/unsigned-gg/herdr-norn) — Synchronized scrollback per project across multiple agent panes.
- [access-tui](https://github.com/unsigned-gg/access-tui) — Live view of connected estate systems and agent channels.
- [toolmon](https://github.com/unsigned-gg/toolmon) — Fleet monitoring of in-house agent tools, versions, and drift across machines.

---

## Deterministic Dispatch & Scheduling

- [ep](https://github.com/unsigned-gg/ep) — Escapement scheduler: metered, deterministic dispatch engine for autonomous agent constellations.
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

Contributions are welcome. Please open an issue or pull request following the guidelines in CONTRIBUTING.md.

---

## License

All software, documentation, and research in this repository are dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
