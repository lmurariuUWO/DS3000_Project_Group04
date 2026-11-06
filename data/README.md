# Data

The dataset is not stored in this repository. Download it yourself:

1. Go to https://universe.roboflow.com/college-whx3b/plant-leaf-diseases
2. Choose version 10 and export in COCO JSON format. Download it as a zip.
3. Unzip so the folder layout is exactly:

```
data/
└── plant_leaf_diseases/
    ├── train/
    │   ├── _annotations.coco.json
    │   └── *.jpg
    ├── valid/
    │   ├── _annotations.coco.json
    │   └── *.jpg
    └── test/
        ├── _annotations.coco.json
        └── *.jpg
```

The notebook reads from `data/plant_leaf_diseases/` using relative paths. Everything under `data/` except this file is git-ignored.
