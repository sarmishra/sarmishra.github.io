Public research projects with companion papers and open-source implementations. All part of a broader agenda on **trustworthy agentic AI** — governance at the reasoning layer, security at the protocol layer, and reliability at the retrieval layer.

---

#### ZT-MCP — Zero-Trust Security for MCP-Connected AI Agents

Zero-trust security architecture for the Model Context Protocol. Four deployable enforcement components — Tool Identity Verifier (TIV), Access Policy Engine (APE), Data Classification and Output Filter (DCOF), and Protocol Audit Logger (PAL) — govern how AI agents access external tools and data. Aligned with NIST SP 800-207 and NIST AI RMF.

<b>Results</b> · 100% attack block rate · 39.5 ms policy enforcement latency · 0% false positive rate on a financial data pipeline prototype

<b>Paper</b> · IEEE COINS 2026 &ensp; <b>Code</b> · [github.com/sarmishra/ZT-MCP-Project](https://github.com/sarmishra/ZT-MCP-Project)

---

#### HITL-AP — Human-in-the-Loop Agentic Pipelines

Seven-layer governance architecture for enterprise deployment of AI agents. An Agentic Oversight Control Plane (AOCP) with policy, risk, and escalation microservices integrates human review into agentic workflows without stalling them. Explicitly complementary to ZT-MCP: HITL-AP governs what the agent decides, ZT-MCP governs how it accesses external infrastructure.

<b>Results</b> · 94% true positive rate · 4.2% false positive rate · p99 latency of 212 ms

<b>Paper</b> · IEEE COINS 2026 &ensp; <b>Code</b> · [github.com/sarmishra/HITL-AP-Project](https://github.com/sarmishra/HITL-AP-Project)

---

#### CHARM — Cascading Hallucination Aware Resolution and Mitigation

Framework for detecting and mitigating cascading hallucinations in agentic RAG pipelines. Introduces a four-type taxonomy for compounding failures across multi-step reasoning, with detection components (SFV, CSCT, CPM, CRT) and a lightweight mitigation loop that operates during agent execution rather than as post-hoc filtering.

<b>Paper</b> · [arXiv:2606.04435](https://arxiv.org/abs/2606.04435) &ensp; <b>Code</b> · [github.com/sarmishra/CHARM-agentic-rag](https://github.com/sarmishra/CHARM-agentic-rag)
