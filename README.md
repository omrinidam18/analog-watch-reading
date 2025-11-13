# Reading Analog Watch Faces with Simple CNN Heads

Author: Omri Nidam (omrinidam@mail.tau.ac.il)  
Affiliation: Tel Aviv University

## Overview
This repository contains the code, trained checkpoints, experiment outputs, and report for reading time from analog watch images using a small supervised model (ResNet-18 + hour/minute heads). It also includes a prompted VLM baseline for comparison.

## Dataset
We use the Synthetic Watch Faces dataset on Hugging Face. The notebook downloads it automatically via `datasets`.

## Repo layout
- `report/` — Final report PDF.
- `notebooks/` — Colab notebook to reproduce all experiments.
- `checkpoints/` — Trained model heads (`.pt`).
- `results/` — CSV/MD summaries, per-image predictions, and reference gallery images.
- `baselines/` — VLM baseline outputs (CSV).

## Quickstart (local)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
# open the notebook in Jupyter or upload to Colab and run end-to-end
