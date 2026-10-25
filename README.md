# Vigyan Sahai

I'm a Computer Science and Mathematics undergraduate in UCSB's College of Creative Studies and a research assistant working on AI for mathematics at UCLA. My interests include reinforcement learning, automated theorem proving, agentic loops, and Mathematics. I would love to gain experience with all aspects of model training.

Some research repositories are private. Public papers, datasets, and code are linked below where available.

## Current Research

### Omega Proof: Reinforcement Learning for Lean Theorem Proving

Developing an AlphaZero-style theorem prover that combines language-model tactic generation, Monte Carlo Tree Search, and a learned value head.

- Designing post-training workflows using SFT and GRPO, alongside synthetic proof-data generation.
- Working with multi-node GPU infrastructure, model serving through vLLM and SGLang, and integration with the slime RL training framework.
- Currently developing parallel MCTS data generation and evaluating how search and learned value estimates can guide proof discovery.

### Updating the Goedel RL dataset to Lean 4.28.0, with corrected formalizations and verified proofs for every theorem in the planned release.

Developing a stronger public dataset of challenging Lean problems for theorem proving and reinforcement learning.

- Corrected roughly 8,000 statements identified as false in the original dataset.
- Checked that statements and proofs compile, and reviewed formalizations for unintended triviality and mismatches with the intended mathematics.
- Adding roughly 10,000 proved problems: 5,000 designed to be easier and 5,000 designed to be harder than their source problems.
- Building proof-generation and multi-round agentic workflows with shared Lean REPL pools and statement/proof correction.

This work is ongoing; final release contents and difficulty evaluations are still being consolidated. Related work includes migrating and auditing miniF2F formalizations against their informal problem statements.

### Agentic Mathematical Research Harnesses

Developing and evaluating systems for long-horizon mathematical research.

- Designing workflows that combine solver, critic, and verifier agents with persistent records of claims, dependencies, and unresolved proof obligations.
- Building research tooling for literature search, computation, and proof-document preparation, including custom MCP integrations.
- Generated candidate proofs for roughly 10 open problems, including Erdős #289, the caterpillar conjecture, and several COLT open problems. Correctness has not been independently established.

## Selected Papers

### TaoBench: Do Automated Theorem Prover LLMs Generalize Beyond MathLib?

Co-author. Findings of EMNLP 2026.

A paired Lean benchmark testing whether theorem-proving models generalize between Tao-style foundational definitions and equivalent Mathlib formulations. My related work includes Lean dataset preparation and parallel proof-verification infrastructure.

Built Lean REPL infrastructure for parallel proof verification and ran model evaluations on the benchmark.

[Paper](https://arxiv.org/abs/2603.12744) · [Project](https://taobench.github.io/) · [Code](https://github.com/ataylor24/TaoAnalysisBench) · [Dataset](https://huggingface.co/datasets/uclanlp/TaoBench)

### Continual Graph Memory for Mathematical Research Agents

Co-author. Under review at ICLR 2027.

Introduces Ansatz, a mathematical research agent using persistent graph memory to organize and reuse reasoning across long research trajectories.

[Paper](https://arxiv.org/abs/2610.02945) · [Code](https://github.com/uclanlp/continual-graph-memory)

## Public AI and Reinforcement Learning Projects

### AlphaZero for the Game of Cycles

- Implemented AlphaZero with MCTS, self-play, and policy/value networks for Tic-Tac-Toe, Connect Four, and the Game of Cycles.
- Used Bayesian optimization to tune training and search hyperparameters, and studied training behavior across iterations.

[Repository](https://github.com/ccs-cs1l-f24/Vigyan-MLProject)

### Geometry Dash AI

- Implemented DQN-based agents using frame observations and reward shaping.
- Built the learning and training components, including architecture and hyperparameter experiments; collaborators handled the game interface and integration.

[Repository](https://github.com/dylanelu/geometry-dash-ai)
