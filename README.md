# TILDA Texture Classification

Kaggle project for MODIA ML 2026: classify grayscale textile texture images from the TILDA dataset into 8 defect categories.

## Dataset

Expected local layout:

```text
data/
  train.csv
  train/
    1.tif
    ...
  test/
    1.tif
    ...
```

The dataset is not committed to Git.

## Approach

- Train models from scratch, without transfer learning or pretrained weights.
- Use moderate data augmentation only on the training split.
- Validate with a stratified split.
- Generate Kaggle submissions with labels converted from internal `0..7` to Kaggle `1..8`.

Main notebook: `notebooks/main_training.ipynb`.

