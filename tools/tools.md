# Frameworks, Tools, and Systems

Overview of core frameworks, architectural paradigms, and software toolkits used to control, verify, and contain error propagation in multi-step agentic AI systems.

---

## 1. Architectural Control Frameworks

### 1. ReAct (Reasoning and Acting)
* **Type:** Architectural Design Pattern / Framework
* **Access Link:** [ReAct Project / Paper](https://arxiv.org/abs/2210.03629)
* **Purpose:** Interleaves internal reasoning traces with external tool action calls.
* **Role in Error Mitigation:** Creates a closed loop (`Plan -> Act -> Observe -> Revise`) that allows external environment feedback to interrupt incorrect internal generation and prevent reasoning drift.

### 2. SELF-RAG (Self-Reflective Retrieval-Augmented Generation)
* **Type:** Adaptive RAG Architecture
* **Access Link:** [Self-RAG Framework](https://arxiv.org/abs/2310.11511)
* **Purpose:** Uses fine-grained reflection tokens (`[Retrieval]`, `[IsRel]`, `[IsSup]`, `[IsUse]`) to critique retrieved passages and generated content on the fly.
* **Role in Error Mitigation:** Separates evidence acquisition from evidence validation, preventing unverified or irrelevant retrieved text from contaminating downstream generation.

### 3. OpenScholar
* **Type:** Retrieval-Augmented Literature Synthesis System
* **Access Link:** [OpenScholar Architecture](https://arxiv.org/abs/2411.14199)
* **Purpose:** Automates scientific literature synthesis using large-scale paper datastores and citation-grounded generation.
* **Role in Error Mitigation:** Maintains strict citation-grounding boundaries to minimize parametric model hallucinations during complex scientific synthesis.

---

## 2. Decision Tree & Search Optimization Tools

### 4. Tree-of-Thoughts (ToT) Framework
* **Type:** Inference Search Paradigm
* **Access Link:** [Tree-of-Thoughts Paper](https://arxiv.org/abs/2305.10601)
* **Purpose:** Enables LLMs to evaluate multiple reasoning branches simultaneously using lookahead and search algorithms (BFS/DFS).
* **Role in Error Mitigation:** Allows agents to detect unpromising reasoning paths early and backtrack before early assumptions corrupt the entire trajectory.

### 5. Graph-of-Thoughts (GoT) Architecture
* **Type:** Network Execution Framework
* **Access Link:** [Graph-of-Thoughts Paper](https://arxiv.org/abs/2308.09687)
* **Purpose:** Models LLM thought generation as an arbitrary graph, allowing aggregation and feedback loops across multiple decision branches.
* **Role in Error Mitigation:** Supports complex error recovery by allowing information from successful sub-branches to correct faulty parallel branches.

### 6. Reflexion Architecture
* **Type:** Verbal Reinforcement Learning Pattern
* **Access Link:** [Reflexion Paper](https://arxiv.org/abs/2303.11366)
* **Purpose:** Uses verbal self-reflection memory to log evaluation feedback after trial attempts.
* **Role in Error Mitigation:** Provides post-failure feedback loops that allow agents to adjust future sub-plans without requiring weight updating or gradient retraining.
```[cite: 1, 2]
