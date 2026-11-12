# DS3000 Project - Group 04: Plant Leaf Disease Classification

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
3. Kernel $\rightarrow$ Restart & Run All.
4. The Stage 2 finalist is saved to 'models/stage2_finalist.joblib' and checked by the smoke-test cell at the end. The file is not committed because of its size. Run the notebook to recreate it.

## Expected runtime
About 30 to 35 minutes on a standard laptop CPU for the full notebook. Most of the time goes to the Stage 2 grid searches, especially AdaBoost (about 18 minutes) and XGBoost (about 6 minutes).

## Project stages
| Stage | Lab | Content | Commit |
|---|---|---|---|
| 1 | Lab 5 (Oct 22) | Data cleaning, EDA, split, baselines (Dummy, LR, SVM, KNN) | `1de973e` (tag `stage1`) |
| 2 | Lab 8 (Nov 12) | MLP, Random Forest, XGBoost, AdaBoost, hyperparameter tuning on validation, model selection (finalist: Random Forest) | tag `stage2` |
| 3 | Lab 11 (Dec 3) | CNN, final test evaluation, analysis | TBD |

## Final commit
TBD
