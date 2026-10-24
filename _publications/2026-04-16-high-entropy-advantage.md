---
title: "High-entropy advantage in neural networks' generalizability"
collection: publications
category: manuscripts
permalink: /publication/2026-04-16-high-entropy-advantage
excerpt: "We treat a neural network as a physical system and compute its Boltzmann entropy landscape with Wang-Landau sampling. Across four tasks (arithmetic, tabular data, image recognition, and language modeling), the high-entropy states generalize as well as or better than SGD-trained networks, and the advantage is larger for narrower networks."
date: 2026-04-16
venue: "npj Artificial Intelligence"
paperurl: "https://doi.org/10.1038/s44387-026-00100-7"
citation: "Yang, E., Zhang, X., <b>Shang, Y.</b>, & Zhang, G. (2026). &quot;High-entropy advantage in neural networks' generalizability.&quot; <i>npj Artificial Intelligence</i>, 2, 44."
---

Why do overparameterized neural networks generalize so well? In this work we take a statistical physics view: each configuration of a network's parameters is a microstate, and the training loss and test accuracy (or test loss) are macroscopic observables. The Boltzmann entropy of a macrostate is then the logarithm of the parameter-space volume that realizes it.

Using Wang-Landau Monte Carlo and Wang-Landau molecular dynamics, we compute these entropy landscapes for four machine learning tasks: a spiral classification problem, Kaggle house-price prediction, a reduced MNIST digit-recognition set, and polymer property prediction with the TransPolymer chemical language model. In all four, the maximum-entropy states at a given training loss generalize at least as well as, and often better than, states reached by SGD training. We call this the *high-entropy advantage*. It weakens as networks get wider, which is consistent with the infinite-width (Gaussian process) limit.

This suggests a thermodynamic explanation for generalization: at low training loss, generalizable solutions occupy far more of parameter space than non-generalizable ones.

Code: [GitHub repository](https://github.com/entao1128/hign_entropy_advantage_NNs/tree/main)
