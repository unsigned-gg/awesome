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
- [Agent Identity & Dynamic Registration](#agent-identity--dynamic-registration)
- [Agent Tooling & Model Context Protocol](#agent-tooling--model-context-protocol)
- [Process Supervision & Systems Core](#process-supervision--systems-core)
- [Deterministic Dispatch & Scheduling](#deterministic-dispatch--scheduling)
- [Sandboxing & Execution Containment](#sandboxing--execution-containment)
- [Contributing](#contributing)
- [License](#license)

---

## The Orchestrator & Autonomous Workforces

- [k8](https://github.com/unsigned-gg/k8) — Kubernetes agent orchestrator, workload controller, and native CLI tooling for autonomous agent fleets.
- [gs](https://github.com/unsigned-gg/gs) — Godseat control surface: operator cluster surface governing perception before action and policy gate tiers.
- [dgr](https://github.com/unsigned-gg/dgr) — Real-time terminal graph renderer: renders autonomous swarm execution DAGs with animated state transitions.
- [herdr](https://github.com/unsigned-gg/herdr) — Autonomous agent session runtime, process coordination, and streaming TTY multiplexer.

---

## Agent Substrates & Runtimes

- [uas](https://github.com/unsigned-gg/uas) — Unsigned Agent Substrate: Rust-native pooled harness runtime with strict zero-I/O domain layering.
- [ls](https://github.com/unsigned-gg/ls) — LeanSpec formal specification engine: zero-I/O AST parser, structural validator, EARS requirement conformance, and 256-bit BLAKE3 CAS listing.

---

## Agent Identity & Dynamic Registration

- [kanidm](https://github.com/kanidm/kanidm) — Fast, memory-safe enterprise identity platform in pure Rust with OAuth2 and OpenID Connect.
- [hydra](https://github.com/ory/hydra) — Headless OAuth2 and OpenID Connect server in Go with native RFC 7591 dynamic client registration.
- [oauth2-test-server](https://crates.io/crates/oauth2-test-server) — In-memory OAuth2 and OpenID Connect server in Rust with native RFC 7591 dynamic registration.
- [openidconnect](https://crates.io/crates/openidconnect) — OpenID Connect crate in Rust supporting RFC 7591 client registration and token discovery.

---

## Agent Tooling & Model Context Protocol

- [rust-sdk](https://github.com/modelcontextprotocol/rust-sdk) — Official Model Context Protocol SDK in Rust for building clients, servers, and agents.
- [hyper-mcp-remote](https://github.com/hyper-mcp-rs/hyper-mcp-remote) — Transport proxy bridging local stdio MCP clients to remote servers via Streamable HTTP with OAuth 2.1.
- [rust-mcp-sdk](https://github.com/rust-mcp-stack/rust-mcp-sdk) — Asynchronous Rust SDK for building MCP clients and servers with stdio and HTTP transports.

---

## Process Supervision & Systems Core

- [kd](https://github.com/unsigned-gg/kd) — Pure-Rust Linux process supervisor using native `pidfd` handles and epoll loops for zombie-free supervision.

---

## Deterministic Dispatch & Scheduling

- [ep](https://github.com/unsigned-gg/ep) — Escapement scheduler: metered, deterministic dispatch engine for autonomous agent swarms (`ep-serve` orchestrator daemon).
- [wak](https://github.com/unsigned-gg/wak) — Accept-and-hold TCP wake proxy and idle reaper for scale-to-zero workloads.

---

## Sandboxing & Execution Containment

- [kl](https://github.com/unsigned-gg/kl) — Kernel Layer primitives: pure-Rust Landlock LSM ruleset compiler, seccomp-BPF system call filtering, and namespace isolation.
- [sbx](https://crates.io/crates/sbx) — AI-containment layer for agent execution: OS syscall jail with reversible run-custody records in Rust.
- [sbxd](https://crates.io/crates/sbxd) — Custody daemon for agent containment: server and orchestrator for Landlock jails.
- [sbx-core](https://crates.io/crates/sbx-core) — Run-custody model: retained changesets and the settle state machine.
- [reach](https://github.com/unsigned-gg/reach) — AI-drivable containerized desktop sandbox.

---

## Contributing

Contributions are welcome. Open an issue or pull request. Follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).

---

## License

All software, documentation, and research in this repository are dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
