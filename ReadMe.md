# Advances in Deep Learning 

Welcome! This repository contains the example notebooks and reference code for the book *Advances in Deep Learning*. The notebooks are organized by chapter (1–13) and include runnable experiments, illustrative visualizations, and short exercises to reinforce concepts from the book.

---

## Prerequisites

- **Python** 3.8+ (conda recommended)
- Jupyter Notebook or JupyterLab
- Common ML packages: `numpy`, `scipy`, `pandas`, `matplotlib`, `scikit-learn` and at least one deep-learning framework such as **PyTorch** or **TensorFlow** depending on the chapter

Tip: Create a virtual environment and install packages with:

```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS / Linux
source venv/bin/activate
pip install jupyterlab numpy scipy pandas matplotlib scikit-learn torch tensorflow
```

If you want, I can generate a `requirements.txt` or `environment.yml` for reproducible environments—ask me to do so.

---

## Quick start

1. Clone the repository:

```bash
git clone <repo-url>
cd Advances-in-Deep-Learning
```

2. (Optional) Create & activate a virtual environment, then install dependencies (see Prerequisites).
3. Start Jupyter:

```bash
jupyter lab
# or
jupyter notebook
```

4. Open the desired notebook, e.g. `chapter-1.ipynb`, and run the cells from top to bottom.

> Note: Some notebooks may take longer to run and might assume GPU availability for large experiments—check the top cells for notes on device configuration.

---

## Repository structure

- `Main_Chapters/` — Core chapter notebooks (`chapter-1.ipynb` … `chapter-13.ipynb`)
- `Bridge_Chapters/` — Supplemental "bridge" notebooks with short, focused examples (`Bridge-chapter-0.ipynb` … `Bridge-chapter-4.ipynb`)
- `ReadMe.md` — This file

---

## Notebook index (quick reference)

Below is a short index of the notebook files grouped by directory. Each entry is a one-line summary of the notebook contents.

### Main_Chapters

- `chapter-1.ipynb` — Toy SSM duality (ToyMambaSSD): demonstrates the equivalence between a scalar state-space model implemented as a recurrent process and as a lower-triangular attention/matrix multiplication, and numerically verifies their outputs.
- `chapter-2.ipynb` — Mixture-of-Experts router: a simple top-k gating/router example that computes router logits, selects top-k experts, and re-normalizes routing weights.
- `chapter-3.ipynb` — Search strategies for reasoning: simulation comparing Greedy (one-shot), Best-of-N, and Tree-Search strategies under constrained compute budgets.
- `chapter-4.ipynb` — Learning internal "thoughts": `ThinkingModel` that samples internal latent 'thoughts' and trains them with a REINFORCE-style signal to improve supervised predictions.
- `chapter-5.ipynb` — Outcome vs Process search (ORM vs PAV): toy environment showing a random outcome-reward search vs a value-based process verifier that looks ahead using an explicit value function.
- `chapter-6.ipynb` — Flow matching (vector field learning): trains a neural vector field to map Gaussian noise to a target "moons" distribution and generates samples via Euler integration.
- `chapter-7.ipynb` — Rectified Flow & distillation: demonstrates 1-rectified and 2-rectified flow training, including reflowing generated pairs and distillation between flows.
- `chapter-8.ipynb` — JEPA-like context encoder & predictor: compresses frames (sine-wave pixel grid) into latents and trains a predictor in latent space to model next-frame dynamics.
- `chapter-9.ipynb` — Conditional flow matching & trajectory generation: trains a velocity field to move noise toward a target distribution and visualizes the generated ODE trajectory.
- `chapter-10.ipynb` — VAR pyramid & coarse-to-fine image generation: simulates multi-scale autoregressive generation by constructing a pyramid of scales from a synthetic image and visualizing predicted scales.
- `chapter-11.ipynb` — Agent S (planner + actor + retrieval): mock filesystem example that illustrates retrieval, high-level planning, and low-level action execution in a simple task loop.
- `chapter-12.ipynb` — Grokking experiment (modular addition): trains an embedding-based model to learn (a + b) mod P and illustrates the memorization → generalization phase transition (grokking).
- `chapter-13.ipynb` — Feature geometry & Simplex ETF: trains a small classifier and analyzes class-means in feature space to check for Simplex Equiangular Tight Frame geometry.

### Bridge_Chapters

- `Bridge-chapter-0.ipynb` — XOR toy: trains a tiny MLP on the XOR problem to demonstrate non-linearity and simple training loop.
- `Bridge-chapter-1.ipynb` — Memory vs Matrix: compares storing low-rank factors vs materialized attention matrix and shows memory & rank implications.
- `Bridge-chapter-2.ipynb` — REINFORCE coin flip: minimal REINFORCE example that learns a Bernoulli policy to favor 'Heads'.
- `Bridge-chapter-3.ipynb` — Adaptive compute simulation: demonstrates allocating more search/compute to high-entropy (uncertain) predictions.
- `Bridge-chapter-4.ipynb` — Best-first search simulation: simple best-first (value-guided) graph search example that finds a path from Start to Goal.

---



