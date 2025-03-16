# Product Summary Dataset

## Overview
This dataset is designed for supervised machine learning tasks, including regression and classification. Users are encouraged to train models on this dataset and evaluate performance using appropriate metrics.

## Dataset Files
- **📂 product_train.csv** – Contains training data with product descriptions and corresponding labels.
- **📂 product_test.csv** – Contains test data with product descriptions only (without labels).

## Preprocessing Steps
1. **Text Cleaning**
   - Removed special characters, numbers, and irrelevant content.
   - Standardized text by converting it to lowercase.

2. **Feature Engineering**
   - Applied TF-IDF Vectorization to convert text into numerical representations.
   - Employed word embeddings (e.g., Word2Vec) for enhanced feature representation.

3. **Dataset Splitting**
   - The dataset was split into 80% training and 20% testing for model evaluation.

## Recommended Approach
1. Train a supervised model using `product_train.csv`.
2. Evaluate the model using `product_test.csv`.
3. Report the following metrics:
   - **Accuracy** (for classification tasks)
   - **F1 Score** (for imbalanced classification tasks)
   - **R-squared (R²)** (for regression tasks)
   - **Mean Squared Error (MSE)** (for regression tasks)

## Column Descriptions

<div align="center">

| Column Name           | Description                                               |
|-----------------------|-----------------------------------------------------------|
| Product Description    | Detailed textual data describing the product features.    |
| Category                | Product category assigned to the item.                   |
| Price                   | Product price information.                               |
| Summary                 | The summarized description generated for each product.   |

</div>

## Category Mapping

<div align="center">

| Category                | Label |
|-------------------------|--------|
| bed_bath_table           | 1      |
| health_beauty            | 2      |
| sports_leisure           | 3      |
| furniture_decor          | 4      |
| computers_accessories    | 5      |
| watches_gifts            | 6      |
| telephony                | 7      |
| garden_tools             | 8      |
| auto                     | 9      |

</div>

## Usage
- Train your supervised learning model using `product_train.csv`.
- Evaluate your model's performance on `product_test.csv` and report accuracy and other metrics.

## Next Steps
- Experiment with various supervised learning models for optimal performance.
- Compare model performance using accuracy, R², F1 Score, or MSE as required.
