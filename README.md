# System-2 AI

Graduate coursework on structured reasoning, neuro-symbolic methods, and large language models, completed during the second semester of my M.Sc. in Computer Engineering at Sharif University of Technology, Spring 2025.

**Instructors:** Dr. Mohammad Hossein Rohban, Dr. Mahdieh Soleymani Baghshah, and Dr. Mohammad Mahdi Samiei.

**Author:** Farzan Rahmani.

## Repository Guide

| Path | Topics and material |
| --- | --- |
| `HWs/HW1/NeuroSymbolic/` | Neuro-symbolic reasoning notebook and CLEVR-related execution/preprocessing utilities |
| `HWs/HW1/Symbolic Regression/` | Symbolic-regression assignment |
| `HWs/HW2/ITS/` | Inference-time scaling: chain of thought, best-of-N, beam search, self-refinement, and search experiments, with saved evaluation JSONs |
| `HWs/HW2/sys2_hw2_rl_post_training_403210725.ipynb` | Reinforcement-learning post-training assignment |
| `HWs/HW3/Graph_RAG/` | GraphRAG implementation for query-focused summarization |
| `HWs/HW3/LLM_Agent/` | LLM-agent assignment |
| `lecture_note/` | Lecture/reference material, including neuro-symbolic sessions |
| `poster session/` | Poster-session instructions, proposal material, and a presentation by Alireza Farajtabrizi and Farzan Rahmani |

## Environment and Usage

Use Jupyter, Google Colab, or another compatible notebook runtime. Each assignment has its own setup cells and dependencies. The inference-scaling notebook installs vLLM, Transformers, Accelerate, and Datasets; GraphRAG uses graph/community libraries and LangChain-related packages.

1. Read the assignment overview and inspect its installation cells before choosing a runtime.
2. Configure datasets, model checkpoints, hosted-runtime paths, and any API authentication.
3. Check GPU support and memory requirements, especially for vLLM and language-model training/inference.
4. Run initialization, experiment, and evaluation cells in order.

vLLM and other accelerated libraries have platform-specific requirements; a native Windows Python environment may not match the original notebooks. External models and datasets may require downloads or access approval. There is no shared lockfile or root application.

## Interpreting Results

The inference-time experiments save results for MATH500 and other test runs. Compare model identifiers, search budgets, scoring rules, prompts, and sampling settings before interpreting differences. GraphRAG explores document processing, graph construction, community detection, and answer synthesis based on the paper *From Local to Global: A GraphRAG Approach to Query-Focused Summarization*.

Saved notebook/JSON outputs document earlier experiments and may not reproduce exactly with changed model services, dependencies, or random seeds.

## License

See [LICENSE](LICENSE) for repository license terms. Course materials, models, papers, and datasets retain their original attribution and terms.
