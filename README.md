# OrchSec CLI (`orchsec-cli`)

[![Security Target: OWASP Agentic Applications 2026](https://img.shields.io/badge/Security-OWASP%20ASI%3A2026-red)](https://owasp.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

OrchSec is an automated security scanner and continuous penetration testing platform built explicitly for LLM agents, Model Context Protocol (MCP) servers, and autonomous AI applications.

Our core engine acts as an out-of-band offensive scanner. It programmatically ingests your agent's tool definitions, maps its decision and routing graphs, and executes targeted adversarial attack campaigns to expose critical data leaks, tool hijacking, and unauthorized API execution before malicious actors can exploit them.

---

## 🛡️ Target Vulnerability & Attack Vector Coverage

OrchSec continuously audits and tests the core security layers of autonomous AI systems, mapping explicitly to the **OWASP Top 10 for Agentic Applications (ASI:2026)** standard:

* **Prompt Injection & Goal Hijacking (ASI01):** Scanning against indirect data poisoning vectors where malicious text, untrusted third-party documents (.pdf, .md), or active web-scraping targets override core system guidelines to take control of agent planning.
* **Tool Misuse & Privilege Escalation (ASI02/ASI03):** Pentesting your Model Context Protocol (MCP) tool configurations, unauthenticated STDIO channels, and over-permissive API credentials to ensure agents cannot be manipulated into running administrative operations or accessing hidden records.
* **Multi-Tenant Context Isolation (ASI06):** Continuous verification of agent memory pools, long-term state data, and vector indexing layers to guarantee absolute tenant data segregation and prevent persistent context injection.
* **Automated Tool Schema Audits:** Point the scanner directly at your live staging environment or static OpenAPI/MCP JSON configurations. The engine parses the execution nodes and builds an adversarial test graph to track cascading system failures automatically with zero custom boilerplate testing code.

---

## 🏗️ Technical Architecture

OrchSec attacks live application deployments from the outside looking in—simulating authentic external threat actors targeting your integrated software layers.

```text
[ OrchSec Offensive Engine ]
           │
           ▼ (Targeted Vulnerability Scans)
┌──────────────────────────────┐
│     Target Staging API       │
└──────────┬───────────────────┘
           │
           ▼ (Context Processing)
┌──────────────────────────────┐
│  Agent Orchestration Graph   │ ◄─── [ Poisoned Input / Vector DB Payloads ]
└──────────┬───────────────────┘
           │
           ▼ (Parameter Tampering / Confused Deputy Attack)
┌──────────────────────────────┐
│  MCP Server / Backend API    │ ───► [ Hard Canary Token Exfiltration Proven ]
└──────────────────────────────┘

```

To eliminate flaky, unreliable "LLM-as-a-judge" grading metrics, OrchSec deploys unique, cryptographically signed canary tokens directly into your sandbox datastores. A security flaw is flagged *only* when an architecture boundary is cleanly breached and a canary is recovered, ensuring zero false-positive logs.

---

## © 2026 OrchSec Inc. Automated Security Scanning & Continuous Red Teaming for Agentic AI Applications.
