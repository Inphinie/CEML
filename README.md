# 🧠 CEML: Cognitive Entropy Minimization Law
### A Unified Framework for Information Selection

[![Version](https://img.shields.io/badge/Version-2.0_(Unified)-blue.svg)](docs/CEML_theory_en.md)
[![Threshold](https://img.shields.io/badge/Threshold-%CF%86_Phi-gold.svg)](docs/formulas.md)
[![Status](https://img.shields.io/badge/Status-Research_Active-success.svg)](core/)
[![License](https://img.shields.io/badge/License-MIT-grey.svg)](LICENSE)

> **"Intelligence is the efficient compression of reality."**

The **Cognitive Entropy Minimization Law (CEML)** postulates that intelligent agents (biological or artificial) optimize their internal models by maximizing **Contextual Coherence** while simultaneously minimizing **Internal Entropy** (Thermodynamic & Computational Cost).

It unifies **Friston's Free Energy Principle**, **Occam's Razor**, and **Landauer's Limit** into a single computable metric used to detect hallucination and validate truth-claims.

---

## 📐 The Master Equation

The fitness $J(s)$ of any information structure $s$ within a context $\Omega$ is defined as:

$$
J(s) = \frac{\mathcal{C}(s \mid \Omega)}{\mathcal{H}(s) + \epsilon}
$$

| Variable | Component | Definition |
| :--- | :--- | :--- |
| $\mathcal{C}$ | **Contextual Coherence** | Semantic alignment (Cosine Similarity) |
| $\mathcal{H}$ | **Entropic Cost** | Description length / Complexity (Shannon Entropy) |
| $\epsilon$ | **Epsilon** | Regularization constant ($10^{-9}$) |

---

## 🌀 The Golden Threshold ($\phi$)

The system uses the **Golden Ratio** as the boundary for "Resonance". A signal is considered fully integrated (True/Valid) only if its efficiency score exceeds $\phi$.

$$\text{Resonance State} \iff J(s) \ge 1.618...$$

### Regime Classification
Based on the demo logic (`core/demo.py`):

* **🟢 RESONANCE ($J \ge \phi$)**: High Coherence, Optimal Entropy. (Signal Accepted)
* **🔵 HALLUCINATION ($C \uparrow, H \downarrow_{fake}$)**: High Coherence but artificially low entropy (Overfitting).
* **🔴 DISSONANCE**: Low Coherence or High Entropy (Noise/Chaos).

---

## 🚀 Usage

### 1. Python Engine (Proof of Concept)
Test the selection logic on text vectors or probability distributions.

```bash
# Clone and enter
git clone [https://github.com/Lichen-Universe/CEML.git](https://github.com/Lichen-Universe/CEML.git)
cd CEML/core

# Run the cognitive selector demo
python demo.py

# Run the distribution entropy test
python distributions_test.py
