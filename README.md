# ResNet Classification Project

This repository contains a Jupyter notebook for ResNet-based image classification and a pretrained model checkpoint.

## Files

- `classification.ipynb` — Jupyter notebook with model definition, training, and evaluation.
- `resnet_cleft_model.pth` — serialized PyTorch model weights. This file is large and should normally be excluded from source control unless you plan to use Git LFS or release it separately.
- `requirements.txt` — Python dependencies for the notebook.

## Setup

1. Create a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook classification.ipynb
```

## Notes

- If you want to upload this repo to GitHub, clear notebook outputs first to avoid bloating the repository and making diffs hard to review.
- The model checkpoint file is 43 MB, which is below GitHub's 100 MB soft limit, but storing binary weights directly in Git is not ideal. Consider removing it from version control and hosting it separately if the repository is intended to stay lightweight.
