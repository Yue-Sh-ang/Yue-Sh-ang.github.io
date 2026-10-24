---
title: "Is Grokking a Computational Glass Relaxation?"
collection: publications
category: conferences
permalink: /publication/2025-12-02-grokking-glass-relaxation
excerpt: "We map grokking onto glass physics: memorization is like rapidly quenching a liquid into a glass, and delayed generalization is like slow relaxation toward equilibrium. Entropy landscapes of transformers show no entropy barrier, so grokking is not a first-order phase transition. A physics-inspired optimizer, WanD, removes grokking without regularization."
date: 2025-12-02
venue: "NeurIPS 2025 (Spotlight)"
paperurl: "/files/grokking-neurips2025.pdf"
citation: "Zhang, X., <b>Shang, Y.</b>, Yang, E., & Zhang, G. (2025). &quot;Is Grokking a Computational Glass Relaxation?&quot; <i>Advances in Neural Information Processing Systems 38 (NeurIPS 2025)</i>."
---

Grokking is the puzzling behavior in which a neural network reaches near-perfect training accuracy long before it generalizes, then suddenly generalizes much later. We study it by treating the network as a physical system: the parameters are the degrees of freedom and the training loss plays the role of energy.

Using Wang-Landau molecular dynamics, we sample the Boltzmann entropy of one-layer transformers on modular arithmetic tasks, as a function of training loss and test accuracy. We find:

- **No entropy barrier** separates the memorizing and generalizing states, and the equilibrium test accuracy varies continuously with training loss. Grokking is therefore not a first-order phase transition.
- **A glass analogy fits the dynamics.** Fast optimization quenches the network into a non-equilibrium, memorizing "computational glass", and grokking is the slow relaxation toward the higher-entropy, generalizing equilibrium.
- **A large high-entropy advantage under grokking.** The gap between trained and maximum-entropy states is much larger than in non-grokking networks, and it shrinks when grokking is suppressed by fixing the weight norm.
- **WanD, a Wang-Landau-based optimizer,** generalizes about as fast as AdamW while largely eliminating grokking. It does so without weight-norm constraints, often reaching high-norm generalizing solutions.

Code: [GitHub repository](https://github.com/xtzhang28/Grokking)

See also the [spotlight poster at NeurIPS 2025](/talks/2025-12-02-neurips-grokking).
