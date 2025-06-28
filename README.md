# Neuro-Symbolic (NeSy) Models

This is a "Giving Back" repository where NeSy models are implemented from scratch in notebook style as a tutorial.



### [DreamCoder](https://dl.acm.org/doi/10.1145/3453483.3454080), ACM-SIGPLAN, 2021

### [Logic Tensor Network](https://arxiv.org/abs/1606.04422), Elsevier AI, 2022

### [Learning Modulo Theories](https://arxiv.org/abs/2301.11435), 2023

### [Differentiable Tree Machine](https://proceedings.mlr.press/v202/soulos23a/soulos23a.pdf), ICML, 2023

### [Data-Efficient Learning with Neural Programs](https://proceedings.neurips.cc/paper_files/paper/2024/hash/1a958c6e813989a0d4b677e6a6f3339a-Abstract-Conference.html), NeurIPS, 2024


---

# Related Work

### [NeuroSymbolic AI: The 3rd Wave](https://arxiv.org/abs/2012.05876), 2020
- **NeuroSymbolic AI (NSAI)** aims to combine symbolic reasoning with deep learning to improve trust, interpretability, and robustness, moving beyond the limitations of purely sub-symbolic models.
- Key challenges include **variable grounding**, **commonsense reasoning**, and extracting **first-order logic (FOL)** from neural networks—difficult due to universal quantifiers violating the universal approximation theorem in bounded continuous spaces.
- **Logic Tensor Networks (LTNs)** provide a framework where constants and variables are embedded as latent vectors and predicates are approximated via neural networks, enabling differentiable reasoning over FOL-like structures.
- NSAI supports **explainability**, **expert knowledge integration**, and bridges **statistical learning** with **knowledge representation and reasoning (KRR)**.
- **Localist vs Distributed representations**: Localist assigns discrete symbols to concepts (e.g., one-hot), while distributed representations encode concepts across many parameters, aiding generalization but limiting interpretability.
- Symbolic knowledge can be encoded in networks via **initialization (compilers)**, **loss constraints**, or **factor graph conversions**, making reasoning differentiable and data-efficient.
- NSAI design combines **gradient descent**, **modularity**, **symbolic languages**, and **constraint satisfaction**; open problems include FOL/higher-order logic extraction, **goal-directed reasoning**, and incorporating **human-in-the-loop** for validating learned representations.

### [The Challenges of Learning Symbolic Representations](https://www.cs.ox.ac.uk/isg/conferences/tmp-proceedings/NeSy2023/paper4.pdf), 2023

- A key challenge is how distributed representations in neural networks can support structured reasoning and symbolic manipulation.
- Reasoning and planning typically require symbolic abstractions, but learning such symbols from perceptual stimuli (e.g., images, audio) is non-trivial. Techniques like VQ-VAE, discrete probabilistic latent spaces, and deep hashing attempt to learn discrete representations for planning, but often fail to ensure **non-ambiguity** and **composability**.
- End-to-end learning of symbolic representations introduces additional difficulties for gradient-based optimization, including issues with **gradient discontinuity**, **temperature annealing**, and **straight-through estimators (STE)**.
- Desired properties of symbolic representations include: **non-ambiguity**, **purity**, **usefulness**, **symbol composability**, **manipulation composability**, and **generalization**.
- Challenges:
  - (a) **Gradient-based optimization**: Approaches such as STE, annealing schedules, and perturbation-based finite differences are used, but remain unstable or brittle.
  - (b) **Loss function choice**: Fuzzy framework etc.
  - (c) **Supervision paradigms**: Vary from fully supervised to unsupervised, including weak or partial signals (e.g., monotonicity constraints, ontologies, or class equivalence).
  - (d) **Knowledge injection strategies**: Include constraints on representations, downstream task constraints (e.g., LatPlan), architectural constraints, semantic regularization, symbolic conditioning, and integration of unstructured knowledge.



