# Belgravia Labs LLC

**Verified Data Infrastructure · Bi-Temporal Knowledge Graphs · Model Context Protocol (MCP) Engines**

[**belgravialabs.com**](https://belgravialabs.com) · [**agenticweb.wiki**](https://agenticweb.wiki) · [**MCP Server (`https://agenticweb.wiki/mcp`)**](https://agenticweb.wiki/mcp) · [**agenticresources.dev**](https://agenticresources.dev) · [**info@belgravialabs.com**](mailto:info@belgravialabs.com)

---

## Overview

Where standard document parsers stop at converting a single file into raw JSON, **Belgravia Labs LLC** builds the **Belgravia Pointer & Ontology Engine (`Stages 01–07`)** — the stateful reasoning and verification layer that resolves messy multi-modal archives and live telemetry streams into:

1. **Time-Aware Bi-Temporal Graphs (`valid_from` / `valid_to` + `observed_at`):** Relational and vector schemas (`PostgreSQL` + `pgvector`) that track both what is true right now and how facts, clauses, or specifications changed over time.
2. **Pointer-Verified Synthesis State (`[P-###]`):** Token-bounded rolling synthesis briefs that eliminate long-context drift while holding hard primary-key and byte-offset pointers back to immutable source records.
3. **Deterministic Constraint Solvers:** Hard-coded rule verifiers (schema, compatibility, spatial, and statutory checks) that gate LLM outputs and score multi-turn agent trajectories.
4. **Two-Way Model Context Protocol (MCP) Surfaces:** High-throughput streamable HTTP MCP servers that serve external AI agents while feeding live query demand back into Stage 01 discovery.

---

## 7-Stage Closed-Loop Architecture

```text
[01] Autonomous Sensor Fleet & Active Probes (Crawlers, Registry Pollers, Live Telemetry)
  │
  ▼
[02] Compliance, Provenance & PII Zoning (Content-Addressed SHA-256 Landing Store + ToS Lineage)
  │
  ▼
[03] Multimodal OCR, Classification & Entity Resolution (Bi-Temporal Relational + Vector Schemas)
  │
  ▼
[04] Bounded Synthesis State & The Pointer Pattern (Token-Bounded Briefs + Hard SQL Pointers)
  │
  ▼
[05] Hierarchical Agent Teams & Observability (Supervisor-Worker Execution + Citation Audit Logs)
  │
  ▼
[06] Verified Synthetic & Contrastive Data Flywheel (Deterministic Verifiers → Evaluation Corpora)
  │
  ▼
[07] Live Domain Instances & Two-Way MCP Surfaces (Serving Agents & Feeding Signal Back to Stage 01)
```

---

## Live Production Domain Instances

Every vertical surface below runs on the same underlying **Belgravia Pointer Engine**:

| Instance | Domain / Surface | Core Engine Capabilities in Production | Status |
| :--- | :--- | :--- | :--- |
| **Instance 01 · AgenticWeb** | [`agenticweb.wiki`](https://agenticweb.wiki)<br>[`agenticresources.dev`](https://agenticresources.dev) | Public protocol discovery registry indexing machine-readable MCP endpoints, `llms.txt`, and Agentic Resource Descriptor (`ard.json`) manifests. Serves **10 live MCP tools** (`define`, `get`, `search`, `has`, `probe`, `changes`, `stale`, `validate_manifest`, `template`, `ask`) and **52 head-to-head benchmarks**. | **Live in Production** (`Cloudflare Workers + D1 + KV`) |
| **Instance 02 · TermsBot** | `TermsBot Compliance Sensor` | Bi-temporal diff engine tracking Terms-of-Service, `robots.txt`, AI training clauses, and API licensing changes with exact byte-offset provenance — powering Stage 02 compliance lineage. | **Private MCP / Enterprise Intake** |
| **Instance 03 · TubeHound** | `@tubehound` / `tubehound.co.uk` | 24/7 high-frequency streaming instance ingesting Transport for London (TfL) network state, planned closures, and headway telemetry to drive an autonomous live broadcast encoder and transit state API. | **Live 24/7 Broadcast & API** |
| **Instance 04 · Sparebay** | `Sparebay Constraint Verifier` | Deterministic **461-rule hardware, ECC memory, and server chassis constraint solver** paired with an autonomous inventory clerk — generating verified tool-use and constraint-satisfaction trajectories for Stage 06. | **Private Engine (`461/461` Tests Passing)** |
| **Instance 05 · TitleMCP** | `TitleMCP Spatial Graph` | Cadastral and spatial instance joining INSPIRE polygons, Price Paid records, and HMLR title registers into an entity-resolved property graph exposed via zero-seat MCP tools. | **Private MCP / Pilot Intake** |

---

## Live MCP Server Quickstart (`agenticweb.wiki/mcp`)

Connect any Model Context Protocol client (Cursor, Claude Desktop, OpenAI Agents SDK, or custom JSON-RPC client) directly to our public discovery and origin-probing engine:

```json
{
  "mcpServers": {
    "agenticweb": {
      "url": "https://agenticweb.wiki/mcp"
    }
  }
}
```

Or query the stateless streamable HTTP MCP endpoint directly via `curl`:

```bash
curl -sS -X POST https://agenticweb.wiki/mcp \
  -H "Content-Type: application/json" \
  -H "Accept: application/json" \
  -d '{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "tools/call",
    "params": {
      "name": "ask",
      "arguments": {
        "question": "Which protocol should I implement to expose machine-readable agent capabilities at my domain root?",
        "use_case": "discovery"
      }
    }
  }'
```

---

## Repository Structure & Open-Data Policy

- **Private Production Repositories:** Core ingestion workers, bi-temporal entity resolution pipelines, deterministic constraint verifiers, and commercial vertical instances are maintained in private repositories under `Belgravia Labs LLC`.
- **Public Specifications, Schemas & Datasets:** Canonical protocol registries, JSON Schemas, executable probe rules, and open benchmark metadata are published in [`Belgravia-Labs/agenticweb-data`](https://github.com/Belgravia-Labs/agenticweb-data) under CC BY 4.0.

---

**Belgravia Labs LLC** · 30 N Gould St, Ste N, Sheridan, WY 82801, USA · [belgravialabs.com](https://belgravialabs.com) · [info@belgravialabs.com](mailto:info@belgravialabs.com)
