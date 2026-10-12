# Rust Model Context Protocol (MCP) Infrastructure

## Overview

The Model Context Protocol (MCP) enables autonomous agents to interact with external tools, contextual resources, and prompt templates across standardized transport boundaries.

In Rust-native agent environments, three core projects provide the foundational SDK, client/server implementations, and remote transport bridges.

---

## 1. Core Implementations

### 1.1 modelcontextprotocol/rust-sdk (Official SDK)

- **Repository:** [github.com/modelcontextprotocol/rust-sdk](https://github.com/modelcontextprotocol/rust-sdk)
- **Primary Function:** The official Model Context Protocol implementation in Rust (`rmcp`).
- **Key Capabilities:**
  - Canonical implementation of the MCP specification in Rust.
  - Asynchronous client and server primitives using Tokio and tracing.
  - Native support for `stdio` and Streamable HTTP transports with OAuth support.
  - Strong schema validation and macro-driven tool definitions.

### 1.2 hyper-mcp-remote

- **Repository:** [github.com/hyper-mcp-rs/hyper-mcp-remote](https://github.com/hyper-mcp-rs/hyper-mcp-remote)
- **Crates.io:** [crates.io/crates/hyper-mcp-remote](https://crates.io/crates/hyper-mcp-remote)
- **Primary Function:** Remote Transport & Authentication Bridge.
- **Key Capabilities:**
  - Bridges local `stdio`-based MCP clients (such as Claude Desktop, Cursor, or Zed) to remote MCP servers using Streamable HTTP.
  - Implements OAuth 2.1 authentication and RFC 7591 Dynamic Client Registration (DCR) for headless agent-to-server authorization.
  - Eliminates the requirement to run heavy tool runtimes directly on the local agent host.

### 1.3 rust-mcp-sdk

- **Repository:** [github.com/rust-mcp-stack/rust-mcp-sdk](https://github.com/rust-mcp-stack/rust-mcp-sdk)
- **Crates.io:** [crates.io/crates/rust-mcp-sdk](https://crates.io/crates/rust-mcp-sdk)
- **Primary Function:** Asynchronous MCP Development Kit.
- **Key Capabilities:**
  - High-performance, asynchronous Rust toolkit for building custom MCP servers and clients.
  - Modular transport layer supporting both `stdio` pipes and Streamable HTTP.
  - Strongly typed protocol message serialization and tool schema validation.

---

## 2. Integration Architecture for UAS and Swarm Lanes

```
+--------------------------------------------------------------+
| Local Agent Lane (herdr / UAS)                                |
|                                                              |
|   +-------------------+      stdio      +------------------+ |
|   | Agent Harness     | --------------> | hyper-mcp-remote | |
|   +-------------------+                 +------------------+ |
+---------------------------------------------------|----------+
                                                    | Streamable HTTP
                                                    | (OAuth 2.1 / DCR)
                                                    v
+--------------------------------------------------------------+
| Remote Tool / Service Node                                    |
|                                                              |
|   +-------------------+                                      |
|   | rmcp / rust-sdk   | (Exposes tools, resources, prompts)  |
|   +-------------------+                                      |
+--------------------------------------------------------------+
```

---

## 3. Specifications & Standards

- Model Context Protocol: [modelcontextprotocol.io](https://modelcontextprotocol.io)
- Official Rust SDK: [github.com/modelcontextprotocol/rust-sdk](https://github.com/modelcontextprotocol/rust-sdk)
- OAuth 2.1 Draft Specification: [datatracker.ietf.org/doc/html/draft-ietf-oauth-v2-1](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-v2-1)
- RFC 7591: [OAuth 2.0 Dynamic Client Registration](https://datatracker.ietf.org/doc/html/rfc7591)
