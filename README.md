# Agentic Development

Architecture and implementation learning resources for building AI agents with LangChain, LangGraph and related technologies.

## AI Data Agent

A three-agent system based on the [Ola AI Data Agent tutorial](https://youtu.be/7yOmi4IX-Rs) and its [reference implementation](https://github.com/anshlambagit/AI_Data_Agent).

| Agent | Responsibility |
| --- | --- |
| SQL Analyst Agent | Interpret questions, construct and validate SQL, execute queries and summarize results |
| ETL Analyst Agent | Select extraction and transformation tools, process API/file data and report results |
| Data Router Agent | Classify user intent and delegate work to the appropriate specialist |

### Architecture and implementation blueprint

**[Read the full AI Data Agent Architecture Blueprint](docs/AI_Data_Agent_Architecture_Blueprint.md)**

The Markdown guide includes Mermaid architecture diagrams, node-by-node execution flows, state contracts, LangChain/LangGraph concepts, Pydantic schemas, tool-calling patterns, implementation guidance for Cursor, and acceptance criteria.

> **Source fidelity:** This is an implementation-oriented reconstruction based on the tutorial transcript and public README. It is not a line-by-line verified reproduction of the reference repository's source files. Verify exact prompts, signatures, graph edges and runtime behavior against the original code before claiming exact parity.

## References

- [Video tutorial](https://youtu.be/7yOmi4IX-Rs)
- [Original AI Data Agent repository](https://github.com/anshlambagit/AI_Data_Agent)
