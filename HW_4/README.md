# Homework 4: Worm Segmentation on BBBC010 (20 pts)

Inverse of HW 3: train a **U-Net (EfficientNet-B0 encoder)** with
[`segmentation_models_pytorch`](https://github.com/qubvel-org/segmentation_models.pytorch)
to predict the foreground mask from a brightfield image.

## Notebooks

* **`00_PrepData.ipynb`** (6 pts, Ex 1) — Download BBBC010, pair brightfield with mask, 80/20 split, save for segmentation
* **`01_TrainModel.ipynb`** (4 pts, Ex 2) — U-Net (EfficientNet-B0), BCE + Dice loss, 30 epochs, save best by val Dice
* **`02_Evaluation.ipynb`** (4 + 6 pts, Ex 3 + Ex 4) — Dice/IoU on test set + best/worst grid; Gaussian-noise robustness sweep + discussion

## Deliverables

1. 3 Jupyter notebooks exported as **HTML**
2. 1-page **PDF report**: final Dice/IoU, best/worst comments, IoU-vs-noise curve and
   deployment-readiness discussion.

## Setup

```bash
uv sync
```

Run notebooks sequentially (00 → 01 → 02). Look for `___` (blanks) and `# TODO:` comments
— those are the parts you need to fill in.
