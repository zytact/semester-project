# AGENTS.md

## Repo shape
- Single artifact: `Speech_Diarization.ipynb` (no package, no scripts, no README/config).

# Project Goal
To create a speech diarization model fine tuned on the AMI dataset.

## Notebook setup (verified from cells)
- Installs deps inside the notebook; use `pip install git+https://github.com/huggingface/diarizers.git` plus `transformers datasets pyannote.audio torch torchaudio accelerate`.
- Pins numpy with `pip install "numpy<2.0.0"` to resolve dependency conflicts in the notebook.
- Uses Hugging Face login via `huggingface_hub.notebook_login()`; HF token improves rate limits.
- Loads dataset `diarizers-community/ami` with config `ihm` via `datasets.load_dataset`.

# WARNING
You cannot run this. This was made to run on Google Colab and nothing is set up locally. Only look at the code.
