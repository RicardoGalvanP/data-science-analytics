# Car Specs: PCA & Exploratory Analysis

Exploratory data analysis and dimensionality reduction using PCA on automobile technical specifications to understand the key drivers of vehicle pricing.

**Status:** EDA and PCA complete. Predictive modeling planned.


### Version

*en: English

*es: Spanish

## Problem Statement

Automobile pricing is influenced by dozens of technical and qualitative features — 
engine specs, dimensions, fuel type, body style, and insurance risk ratings. This 
project applies Principal Component Analysis (PCA) to reduce dimensionality, 
identify the most meaningful feature combinations, and understand the variance 
structure driving car prices.

## Dataset

- **Source:** UCI Machine Learning Repository — Automobile Dataset
- **Key Features:**
  - `make` — Brand (Audi, BMW, Honda, etc.)
  - `fuel_type`, `aspiration`, `body_style`, `drive_wheels` — Vehicle specs
  - `engine_type`, `num_cylinders`, `engine_size`, `horsepower` — Engine specs
  - `curb_weight`, `length`, `width`, `height`, `wheel_base` — Dimensions
  - `city_mpg`, `highway_mpg` — Fuel efficiency
  - `symboling` — Insurance risk rating (-3 to +3)
  - `normalized_losses` — Normalized insurance losses
- **Target:** `price` (USD)

## Tech Stack

- Python 3.9
- Pandas, NumPy
- Scikit-learn (PCA, StandardScaler, SimpleImputer, OneHotEncoder)
- Matplotlib, Seaborn
- Google Colab

## Methodology

1. **Data Cleaning** — Handled missing values using SimpleImputer, removed 
   inconsistencies
2. **EDA** — Explored relationships between features and price using 
   correlation analysis and visualizations
3. **Preprocessing** — Encoded categorical variables, scaled numerical features
4. **PCA** — Applied Principal Component Analysis to reduce dimensionality

## Key Results

| Principal Component | Variance Explained |
|---|---|
| PC1 | 45% |
| PC2 | 18% |
| PC3 | 9% |
| PC4 | 6% |
| PC5 | 6% |

The first 2 components explain **63% of total variance**, and the first 5 
components capture **84%** — significantly reducing the feature space while 
retaining most of the data's information structure.

## What I Learned

- How to handle real-world messy data with missing values and mixed types
- Applying PCA to high-dimensional datasets and interpreting eigenvalues
- How dimensionality reduction reveals hidden structure in automotive data
- Trade-offs between number of components and variance retained
