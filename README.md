<div align="center">

# Aman Raj Verma

**Backend systems · Distributed applications · AI agents**

Building with Java, Spring Boot, and Python.

**Portfolio: [arv0007.github.io](https://arv0007.github.io)** · [Resume](https://arv0007.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/arv14)

| Project | Live demo | Code |
| :--- | :--- | :--- |
| ForgeFlow, AI app builder | [forgeflow-7m08.onrender.com](https://forgeflow-7m08.onrender.com) | [repo](https://github.com/ARV0007/forgeflow) |
| Transakt, payment gateway | [Try it in your browser](https://arv0007.github.io/transakt/) | [repo](https://github.com/ARV0007/transakt) |
| Transakt Sentinel, fraud agent | [Replay a recorded run](https://arv0007.github.io/sentinel/) | [repo](https://github.com/ARV0007/transakt-sentinel) |

</div>

---

I build applications that connect backend engineering with practical AI. My projects explore payment reliability, event-driven workflows, and agents that use tools, validate their work, and pause for human review.

## Selected work

### ForgeFlow — from a prompt to a working app

An AI app builder with conversational edits, live previews, and version history. The generation loop checks the build and feeds errors back to the agent for repair.

- **Agent workflows:** planning, targeted file edits, review, and visual checks.
- **Retrieval:** hybrid code search with vector and full-text retrieval.
- **Platform:** streaming responses, project sharing, and deployment options.

**Built with:** Java · Spring Boot · PostgreSQL · pgvector · Redis · Qdrant

[Open the live app](https://forgeflow-7m08.onrender.com) · [Explore the code](https://github.com/ARV0007/forgeflow) · [Architecture](https://github.com/ARV0007/forgeflow/blob/main/docs/architecture.md)

### Transakt — payment processing with explicit failure handling

A payment gateway project with merchant APIs and double-entry ledger accounting. Its design addresses duplicate requests, uncertain bank responses, and reliable event delivery.

- **Correctness:** idempotent payment requests and ledger entries.
- **Recovery:** reconciliation for payments with an unknown outcome.
- **Events:** a transactional outbox feeding Kafka webhooks with retries and a dead-letter path.

**Built with:** Java · Spring Boot · PostgreSQL · Redis · Apache Kafka

[Try it in your browser](https://arv0007.github.io/transakt/) · [Explore the code](https://github.com/ARV0007/transakt) · [Design decisions](https://github.com/ARV0007/transakt/blob/main/docs/notes.md)

### Transakt Sentinel — fraud investigation with human review

A companion system that scores payment risk with ML and investigates flagged cases through an AI agent. The agent gathers evidence and recommends an action; a human analyst makes the decision.

- **Risk scoring:** a fast ML model processes payment events.
- **Investigation:** LangGraph workflows gather evidence through MCP tools.
- **Operations:** durable checkpoints, replay handling, and monitoring.

**Built with:** Python · FastAPI · LangGraph · scikit-learn · Kafka · Redis

[Replay a recorded run](https://arv0007.github.io/sentinel/) · [Explore the code](https://github.com/ARV0007/transakt-sentinel)

## Tools I use

| Area | Technologies |
| :--- | :--- |
| Backend | Java, Spring Boot, Spring Security, Python, FastAPI |
| Data & messaging | PostgreSQL, Redis, Apache Kafka, pgvector, Qdrant |
| AI & ML | LangGraph, LangChain, scikit-learn, RAG, MCP |
| Delivery & testing | Docker, GitHub Actions, Maven, JUnit |
| Web | HTML, CSS, JavaScript |

## How I approach engineering

**Design for failure.** Make retries safe, preserve state, and make errors understandable.

**Test the boundaries.** Check behavior where services, databases, and external systems meet.

**Keep AI accountable.** Use validation checks, evidence, and human review where decisions need it.

**Explain the trade-offs.** Keep architecture notes, setup instructions, and known limitations alongside the code.

---

<sub>Project READMEs include implementation details, tests, and current limitations.</sub>
