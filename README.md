# AI Data Agent System Blueprint

**Delivered by:** [Zynx Technologies Ltd](https://www.zynxtechnologies.com/)  
**Portfolio host (pre-fork):** `anoopdk/Agentic-Development`  
**Domain client (sanitised):** Zynx x Digital / AI Client  
**Engagement type:** Solution Architecture Delivery  
**Portfolio version:** `1.0.0-portfolio`

> Inspection note: Client identity is domain-aliased for public portfolio use. This repository is structured for authenticity review of delivery artefacts, architecture, and engagement scope.

## Project overview

The Digital / AI Client wanted an agentic analytics pattern where natural-language questions can be routed to specialised SQL or ETL agents with explicit state contracts, validation, and human-governed implementation guidance.

### Solution delivered

Zynx delivered an architecture blueprint for a three-agent system (SQL Analyst, ETL Analyst, Data Router) with Mermaid flows, LangChain/LangGraph guidance, schema contracts, and acceptance criteria suitable for Cursor-assisted implementation.

## Engagement levels

| # | Level |
| --- | --- |
| 1 | Capability Discovery |
| 2 | Multi-Agent Architecture |
| 3 | State / Tooling Contracts |
| 4 | Implementation Guidance Pack |

| Field | Value |
| --- | --- |
| Engagement posture | Delivery portfolio artefact prepared for audit / inspection |
| Confidentiality | Domain alias only; no real client legal name in public docs |
| Primary artefacts | Code/notebooks/docs already in-repo + Zynx standard pack under `docs/` and `decks/` |

## Architecture

```mermaid
flowchart TB
  U[User question] --> R[Data Router Agent]
  R -->|SQL intent| S[SQL Analyst Agent]
  R -->|ETL / file / API intent| E[ETL Analyst Agent]
  S --> ANS[Summarised answer]
  E --> ANS
```

### Implementation flow

```mermaid
flowchart LR
  BP[Architecture blueprint] --> SC[State contracts]
  SC --> TOOLS[Tool-calling patterns]
  TOOLS --> ACC[Acceptance criteria]
```

## Technology stack

`LangChain`, `LangGraph`, `Pydantic schemas`, `SQL + ETL tool calling`, `Mermaid architecture`

## Repository map

| Path | Purpose |
| --- | --- |
| `README.md` | Project overview + engagement levels |
| `docs/` | Problem, solution, architecture, implementation, runbook, audit factsheet |
| `decks/` | 3-slide delivery overview (Markdown + HTML) |
| `src/` / project subtree | Implementation assets (or placeholders where design-led) |
| `tests/` | Tests or placeholders |
| `scripts/` | Operational / helper scripts |
| `configs/` | Non-secret configuration templates |
| `.env.example` | Environment variable placeholders |

### Key existing delivery paths

- `docs/AI_Data_Agent_Architecture_Blueprint.md`

## How to inspect this repository

1. Read this README (overview + engagement).
2. Open `docs/audit/PROJECT-FACTSHEET.md`.
3. Review architecture in `docs/03-architecture.md`.
4. Walk implementation evidence listed in the factsheet.
5. Open `decks/overview.html` for the 3-slide executive summary.

## Related Zynx context

Zynx Technologies Ltd provides IT consulting across cloud, data analytics, and digital delivery. This repository is part of the public delivery portfolio hosted on `anoopdk` prior to organisation-level fork.

## License

See `LICENSE`.
