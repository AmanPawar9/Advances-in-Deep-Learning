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

- `chapter-1.ipynb` — `chapter-13.ipynb`: Example notebooks for Chapters 1–13
- `ReadMe.md`: This file

---

## Notebook index (quick reference)

Below is a short index of the notebook files. Each notebook contains runnable code and short explanations aligned with the corresponding chapter in the book.

- `chapter-1.ipynb` — Introduction, notation, and setup examples
- `chapter-2.ipynb` — Supervised learning basics and small-scale experiments
- `chapter-3.ipynb` — Neural network fundamentals and training loops
- `chapter-4.ipynb` — Optimization methods and practical tips
- `chapter-5.ipynb` — Regularization and generalization experiments
- `chapter-6.ipynb` — Convolutional architectures and image tasks
- `chapter-7.ipynb` — Sequence models and recurrent networks
- `chapter-8.ipynb` — Attention mechanisms and transformers
- `chapter-9.ipynb` — Generative models and VAEs/GANs
- `chapter-10.ipynb` — Reinforcement learning basics & experiments
- `chapter-11.ipynb` — Scaling up models and distributed training notes
- `chapter-12.ipynb` — Advanced optimization, second-order methods
- `chapter-13.ipynb` — Case studies, reproducibility, and research pointers


