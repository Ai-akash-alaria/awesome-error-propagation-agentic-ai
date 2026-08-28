# Open-Source Repositories & Implementations

A curated list of high-quality open-source GitHub repositories containing production-ready implementations, process supervision tools, and trajectory debugging code bases relevant to agentic reliability.

---

## 1. Verified Implementations

### 1. ReAct Implementation (`princeton-nlp/ReAct`)
* **Repository:** [https://github.com/princeton-nlp/ReAct](https://github.com/princeton-nlp/ReAct)
* **Maintained By:** Princeton NLP Group
* **Description:** Official implementation of the ReAct paradigm combining reasoning traces and action generation for agentic task execution.
* **Relevance:** Provides the base execution loop for tool-calling agents and environment state management.

### 2. Self-RAG Framework (`AkariAsai/self-rag`)
* **Repository:** [https://github.com/AkariAsai/self-rag](https://github.com/AkariAsai/self-rag)
* **Maintained By:** OpenScholar / UW NLP Authors
* **Description:** Complete code base for training and inference with Self-RAG reflection tokens and adaptive retrieval filters.
* **Relevance:** Demonstrates how to programmatically filter out low-confidence or hallucinated retrieved passages before passing them downstream.

### 3. Tree-of-Thought LLM (`princeton-nlp/tree-of-thought-llm`)
* **Repository:** [https://github.com/princeton-nlp/tree-of-thought-llm](https://github.com/princeton-nlp/tree-of-thought-llm)
* **Maintained By:** Princeton NLP Group
* **Description:** Official repository for search over reasoning trees (BFS/DFS) using language models as evaluators and generators.
* **Relevance:** Crucial reference code for building agentic architectures capable of backtracking on error detection.

### 4. Graph-of-Thoughts Engine (`spcl/graph-of-thoughts`)
* **Repository:** [https://github.com/spcl/graph-of-thoughts](https://github.com/spcl/graph-of-thoughts)
* **Maintained By:** Scalable Parallel Computing Lab (ETH Zurich)
* **Description:** Executable framework for graph-structured LLM reasoning, transformation, and feedback loops.
* **Relevance:** Enables non-linear agent workflow execution with error containment across multi-branch dependencies.

### 5. OpenAI PRM800K Resources (`openai/prm800k`)
* **Repository:** [https://github.com/openai/prm800k](https://github.com/openai/prm800k)
* **Maintained By:** OpenAI
* **Description:** Data utilities, schema definitions, and model evaluation routines for step-level process supervision.
* **Relevance:** Provides structural guidelines for implementing step-level verifier models in agentic research workflows.

---

## 2. Selection Criteria Met

All listed repositories were selected based on:
1. **Direct Literature Connection:** Tied directly to peer-reviewed research papers cited in this repository[cite: 1, 2].
2. **Maintenance & Open Access:** Clean, readable open-source codebases under permissive licenses (MIT / Apache 2.0)[cite: 1].
3. **Reproducibility:** Code repositories include execution scripts, dataset loaders, and documentation[cite: 1].
```[cite: 1, 2]
