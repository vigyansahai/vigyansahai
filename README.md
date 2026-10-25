# Vigyan Sahai

I'm a Computing and Mathematics undergraduate in UCSB's College of Creative Studies and a research assistant working on AI for mathematics at UCLA. My interests include reinforcement learning, automated theorem proving, mathematical research agents, and the systems that make large-scale experiments possible.

Some research repositories are private. Public papers, datasets, and code are linked below where available.

## Current Research

### Omega Proof: Reinforcement Learning for Lean Theorem Proving

Developing an AlphaZero-style theorem prover that combines language-model tactic generation, Monte Carlo Tree Search, and a learned value head.

- Building proof-search and value-training workflows around persistent pools of Lean REPLs.
- Designing post-training workflows using SFT and GRPO, alongside synthetic proof-data generation.
- Working with multi-node GPU infrastructure, model serving through vLLM and SGLang, and integration with the slime RL training framework.
- Currently developing parallel MCTS data generation and evaluating how search and learned value estimates can guide proof discovery.

### Updating the Goedel RL Dataset

Developing a stronger public dataset of challenging Lean problems for theorem proving and reinforcement learning.

- Updating Lean statements and proof-generation infrastructure, with an emphasis on preserving the intended mathematics during migration and repair.
- Reviewing formalizations for unintended shortcuts, inconsistent assumptions, and other defects that can make a problem misleadingly easy.
- Building resumable proof-generation and verification workflows with shared Lean REPL pools, statement/proof tracking, and checks for admissions and unexpected axioms.
- Exploring synthetic theorem variants intended to vary difficulty. Proof validity, semantic fidelity, and measured difficulty are separate evaluation goals.

This work is ongoing; final release contents and difficulty evaluations are still being consolidated. Related work includes migrating and auditing miniF2F formalizations against their informal problem statements.

### Agentic Mathematical Research Harnesses

Developing and evaluating systems for long-horizon mathematical research, including MoonshotMath and MoonshotMathv2.

- Designing workflows that combine solver, critic, and verifier agents with persistent records of claims, dependencies, and unresolved proof obligations.
- Building research tooling for literature search, computation, and proof-document preparation, including custom MCP integrations.
- Comparing harness designs and organizing research outputs with explicit verification status rather than treating generated solutions as established results.

## Selected Papers

### TaoBench: Do Automated Theorem Prover LLMs Generalize Beyond MathLib?

Co-author. Findings of EMNLP 2026.

A paired Lean benchmark testing whether theorem-proving models generalize between Tao-style foundational definitions and equivalent Mathlib formulations. My related work includes Lean dataset preparation and parallel proof-verification infrastructure.

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

## Technical Interests

Reinforcement learning · Monte Carlo Tree Search · LLM post-training · Lean verification · Agent evaluation · Distributed GPU systems
