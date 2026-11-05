# DSC180A Pain Axis Reproduction

UC San Diego DSC 180A Capstone project. We are working on a preliminary reproduction of [*The Pain Axis* (Tagliabue et al., 2026)](https://arxiv.org/abs/2609.16247), exploring pain-related representations in language models and how activation steering affects model behavior.

## Notebooks

- **`01_pain_axis.ipynb`** — Load the original dataset, extract activations using Qwen2.5-0.5B, compute an initial pain direction with difference-in-means, and apply PCA denoising.
- **`02_validation.ipynb`** — Evaluate pain-direction classification with cross-validation, compare layers, and test against fear, sadness, and other controls.
- **`03_steering_and_button.ipynb`** — Explore activation steering and simulated button-choice experiments using Qwen2.5-7B-Instruct.

## Data and running the code

The notebooks load data from the [authors' Pain Axis repository](https://github.com/valen-research/Pain-axis). Models are loaded from Hugging Face. Run the notebooks in numerical order with a Python/Jupyter environment and packages such as PyTorch, Transformers, NumPy, pandas, scikit-learn, and Matplotlib. GPU access is recommended; the 7B experiments use 4-bit quantization and require additional packages such as `bitsandbytes` and `accelerate`.

These are **preliminary experiments**, not yet a complete reproduction of the paper.

## AI assistance

AI tools, including ChatGPT and Codex, were used during the reproduction process to brainstorm approaches, clarify methods, suggest code, and help debug issues. The team remains responsible for checking the implementation and interpreting the experimental results.
