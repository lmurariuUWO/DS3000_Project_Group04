# DS3000 Project — Group 04: Plant Leaf Disease Classification

## Problem
Predict the plant/disease category of a leaf image using supervised multiclass image classification. Each observation is one image containing exactly one distinct annotated category. Images with no label or with multiple distinct categories are excluded.

## Dataset
- Source: Plant Leaf Diseases, License: CC BY 4.0, Roboflow Universe - https://universe.roboflow.com/college-whx3b/plant-leaf-diseases (dataset #16)

- Version: v10, COCO JSON export

- Provided split: train 3426 / valid 428 / test 428 images (≈80/10/10). We keep this split.

- For raw data download and placement see [`data/README.md`](data/README.md).

## Setup
Python 3.12.

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Run order
1. Download the dataset and follow `data/README.md` for placement.
2. Open `DS3000_Project_Group04.ipynb`.
3. Kernel → Restart & Run All.

## Expected runtime
About 1.50 to 2.00 minutes on a standard laptop CPU (Stage 1). Most of the time goes to image loading and feature extraction plus the SVM fit (about 20 s).

## Project stages
| Stage | Lab | Content | Commit |
|---|---|---|---|
| 1 | Lab 5 (Oct 22) | Data cleaning, EDA, split, baselines (Dummy, LR, SVM, KNN) | `1de973e` |
| 2 | Lab 8 (Nov 12) | MLP, tree-based models, HPO on validation, model selection | TBD |
| 3 | Lab 11 (Dec 3) | CNN, final test evaluation, analysis | TBD |

## Final commit
TBD
