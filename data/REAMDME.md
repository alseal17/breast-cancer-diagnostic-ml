# Dataset Information

This project uses the **Enhanced Breast Cancer Diagnostic Dataset**, which contains diagnostic tumor measurements used to classify breast tumors as **benign** or **malignant**.

The dataset was downloaded directly from Kaggle using the `kagglehub` Python package.

## Original Dataset

**Enhanced Breast Cancer Diagnostic Dataset**

https://www.kaggle.com/datasets/shivasingh4945/enhanced-breast-cancer-diagnostic-dataset

## Dataset Description

The dataset contains diagnostic measurements describing tumor morphology, including features such as:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Concave Points
- Shape Irregularity
- Border Complexity

The target variable is:

- **B** = Benign
- **M** = Malignant

Several engineered interaction features are also included.

## Data Usage

The dataset is **not included** in this repository to respect the original creator's distribution and licensing.

To reproduce this project:

1. Download the dataset from the Kaggle link above.
2. Place the dataset in this `data/` directory or download it programmatically using `kagglehub`.
3. Run the notebook in the `notebooks/` folder.

## Attribution

Dataset created and published by **shivasingh4945** on Kaggle.

If you use this dataset, please consider citing or acknowledging the original author on Kaggle.
