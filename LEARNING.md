# Makemore learning track

This fork retains Andrej Karpathy's original `makemore.py`, `names.txt`, `README.md` and `LICENSE`.
The added materials are an **independent learning workspace**, not a maintained replacement for upstream.

## Learning sequence

- [01-bigrams](notebooks/01-bigrams.ipynb) — Character vocabulary and count-based bigrams
- [02-neural-bigrams](notebooks/02-neural-bigrams.ipynb) — Neural bigrams and gradients
- [03-embeddings-mlp](notebooks/03-embeddings-mlp.ipynb) — Embeddings and multilayer perceptrons
- [04-backpropagation](notebooks/04-backpropagation.ipynb) — Backpropagation from first principles
- [05-training](notebooks/05-training.ipynb) — Training, evaluation and reproducibility
- [06-transformers](notebooks/06-transformers.ipynb) — From context windows to attention

These notebooks contain **objectives, starter setup and space for exercises**, not worked solutions.
The tutorial sequence is a learning scaffold rather than a claim that upstream supplies these notebooks.

## Colab

1. Open a notebook in `notebooks/` on GitHub and choose **Open in Colab**, or open its GitHub URL from Colab.
2. Use a Python runtime to begin with. Choose Runtime → Change runtime type → GPU when needed.
3. Run the notebook's clone cell to fetch the reference `names.txt` and `makemore.py`.
4. Use Gemini Learn Mode to discuss derivations, inspect tensor shapes, and diagnose mistakes.
5. Save notebook edits back to this GitHub fork using Colab's GitHub save option. Prefer a separate work branch.

**Important:** Colab runtime storage is temporary; preserve important outputs before the runtime disconnects. GPU availability and limits are controlled by Google. GitHub commits made after a Colab session starts do not automatically update its cloned working tree.

## Local or Solveit

Use a Python 3 environment with PyTorch installed. Follow the [PyTorch installation selector](https://pytorch.org/get-started/locally/) for your machine, especially for CUDA. No GPU is necessary for early exercises.

The local working directory and the Colab clone directory can differ; use explicit paths instead of assuming that notebook working directories are the repository root.

## Reproducibility checklist

Record: upstream/fork commit SHA; Python and PyTorch versions; hardware; random seed; train/dev/test split; hyperparameters; and observed results. Do not assume reproducibility across different hardware or CUDA kernels.

## Repo boundaries

- Original upstream files stay in the repository root.
- `notebooks/` is for one learning stage per notebook.
- `experiments/` is for later independent investigations.
- Outputs, large model weights, credentials and transient runtime files must not be committed.
- Retain the original MIT license and attribution.

Reference upstream: https://github.com/karpathy/makemore
