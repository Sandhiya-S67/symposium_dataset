# Product Summary Dataset

## Overview
This dataset is designed for supervised machine learning tasks, including regression and classification. Users are encouraged to train models on this dataset and evaluate performance using appropriate metrics.

## Dataset Files
- **📂 product_train_labels.csv** – 80% of the dataset used for training purposes with encoded category labels (1 to 9).
- **📂 product_test_labels.csv** – 20% of the dataset used for testing purposes with encoded category labels (1 to 9).

## Preprocessing Steps
1. **Text Cleaning**
   - Removed special characters, numbers, and irrelevant content.
   - Standardized text by converting it to lowercase.

2. **Feature Engineering**
   - Applied TF-IDF Vectorization to convert text into numerical representations.
   - Employed word embeddings (e.g., Word2Vec) for enhanced feature representation.

3. **Dataset Splitting**
   - The dataset was split into 80% training and 20% testing for model evaluation.

4. **Label Encoding**
   - Product categories were encoded into 9 distinct numerical labels.

## Recommended Approach
1. Train a supervised model using `product_train_labels.csv`.
2. Evaluate the model using `product_test_labels.csv`.
3. Report the following metrics:
   - **Accuracy** (for classification tasks)
   - **F1 Score** (for imbalanced classification tasks)
   - **R-squared (R²)** (for regression tasks)
   - **Mean Squared Error (MSE)** (for regression tasks)

## Column Descriptions
| Column Name | Description |
|--------------|--------------|
| Product Description | Detailed textual data describing the product features. |
| Category | Encoded product category labels (ranging from 1 to 9). |
| Price | Product price information. |
| Summary | The summarized description generated for each product. |

## Usage
- Train your supervised learning model using `product_train_labels.csv`.
- Evaluate your model's performance on `product_test_labels.csv` and report accuracy and other metrics.

## Next Steps
- Experiment with various supervised learning models for optimal performance.
- Compare model performance using accuracy, R², F1 Score, or MSE as required.

