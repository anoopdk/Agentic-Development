# Architecture

## Context diagram

```mermaid
flowchart TB
  U[User question] --> R[Data Router Agent]
  R -->|SQL intent| S[SQL Analyst Agent]
  R -->|ETL / file / API intent| E[ETL Analyst Agent]
  S --> ANS[Summarised answer]
  E --> ANS
```

## Implementation flow

```mermaid
flowchart LR
  BP[Architecture blueprint] --> SC[State contracts]
  SC --> TOOLS[Tool-calling patterns]
  TOOLS --> ACC[Acceptance criteria]
```

## Design notes

- Prefer layered medallion / governed platform patterns where applicable.
- Keep configuration and secrets outside Git.
- Preserve auditability: documentation must match repository evidence.
