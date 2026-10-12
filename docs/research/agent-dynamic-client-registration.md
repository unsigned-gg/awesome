# Agent Identity & Dynamic Client Registration (RFC 7591)

## Overview

In autonomous multi-agent environments, agents require programmatic, headless mechanisms to obtain authentication credentials, register client identities, and access network services without manual human intervention.

This specification documents the open-source and Rust ecosystem implementations of **RFC 7591 (OAuth 2.0 Dynamic Client Registration Protocol)**, workload identity patterns, and emerging Model Context Protocol (MCP) authentication conventions.

---

## 1. RFC 7591 Wire Specification

RFC 7591 standardizes programmatic client creation via HTTP `POST` requests to an authorization server's registration endpoint.

### Registration Request (`POST /oauth2/register`)

```http
POST /oauth2/register HTTP/1.1
Host: auth.example.com
Authorization: Bearer <INITIAL_ACCESS_TOKEN>
Content-Type: application/json

{
  "client_name": "agent-thuban-runner",
  "redirect_uris": [
    "https://agent.unsigned.gg/oauth/callback"
  ],
  "grant_types": [
    "client_credentials",
    "authorization_code"
  ],
  "response_types": [
    "code"
  ],
  "token_endpoint_auth_method": "client_secret_basic",
  "scope": "openid profile read:code write:reports"
}
```

### Registration Response (`HTTP/2 201 Created`)

```json
{
  "client_id": "c7f91a2b-3c4d-5e6f-7a8b-9c0d1e2f3a4b",
  "client_secret": "sec_9x8w7v6u5t4s3r2q1p0o_hash",
  "client_id_issued_at": 1791775000,
  "client_secret_expires_at": 0,
  "registration_client_uri": "https://auth.example.com/oauth2/register/c7f91a2b",
  "registration_access_token": "reg_token_abc123"
}
```

---

## 2. Open-Source Ecosystem Implementations

### 2.1 Pure-Rust Implementations

| Project | License | Source | Description |
|---|---|---|---|
| **Kanidm** | MPL-2.0 | [github.com/kanidm/kanidm](https://github.com/kanidm/kanidm) | Pure-Rust enterprise identity platform with OAuth2, OIDC, WebAuthn, and API client provisioning. |
| **Matrix Authentication Service** | Apache-2.0 | [github.com/matrix-org/matrix-authentication-service](https://github.com/matrix-org/matrix-authentication-service) | Standalone OIDC provider in Rust using Axum and SQLx with strict RFC conformance. |
| **oauth2-test-server** | MIT / Apache-2.0 | [crates.io/crates/oauth2-test-server](https://crates.io/crates/oauth2-test-server) | In-memory OAuth2/OIDC server in Rust with native RFC 7591 dynamic registration. |
| **openidconnect** | MIT / Apache-2.0 | [crates.io/crates/openidconnect](https://crates.io/crates/openidconnect) | Comprehensive OpenID Connect client and server primitives in Rust with RFC 7591 support. |
| **auth-framework** | MIT / Apache-2.0 | [crates.io/crates/auth-framework](https://crates.io/crates/auth-framework) | Pluggable auth framework with dynamic registration handlers for Axum. |

### 2.2 Go and Enterprise Implementations

| Project | License | Source | Description |
|---|---|---|---|
| **Ory Hydra** | Apache-2.0 | [github.com/ory/hydra](https://github.com/ory/hydra) | Headless OAuth2/OIDC server in Go with native RFC 7591 dynamic client registration. |
| **Zitadel** | Apache-2.0 | [github.com/zitadel/zitadel](https://github.com/zitadel/zitadel) | Cloud-native multi-tenant IAM platform in Go supporting RFC 7591. |
| **Keycloak** | Apache-2.0 | [github.com/keycloak/keycloak](https://github.com/keycloak/keycloak) | Enterprise Java identity broker with native Dynamic Client Registration. |

---

## 3. Emerging Trends: Client ID Metadata Documents (CIMD)

In decentralized agent networks and Model Context Protocol (MCP) ecosystems:

1. **Centralized Registration Limitations:** Centralized RFC 7591 databases create single points of coordination across cross-organizational agent swarms.
2. **Client ID as URL:** Emerging standards (such as ATProto OAuth and MCP remote specs) transition toward **Client ID Metadata Documents (CIMD)**.
3. **Decentralized Discovery:** The `client_id` is an HTTPS URL resolving directly to a signed JSON metadata document hosted by the agent. The authorization server fetches the document dynamically, verifying cryptographic origin without requiring prior registration.

---

## 4. References & Specifications

- IETF RFC 7591: [OAuth 2.0 Dynamic Client Registration Protocol](https://datatracker.ietf.org/doc/html/rfc7591)
- IETF RFC 7592: [OAuth 2.0 Dynamic Client Registration Management Protocol](https://datatracker.ietf.org/doc/html/rfc7592)
- OpenID Foundation: [OpenID Connect Dynamic Client Registration 1.0](https://openid.net/specs/openid-connect-registration-1_0.html)
