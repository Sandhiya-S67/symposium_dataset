# Product Summary Dataset

## Overview
This dataset is designed for supervised machine learning tasks, including regression and classification. Users are encouraged to train models on this dataset and evaluate performance using appropriate metrics.

## Dataset Files
- **📂 product_train.csv** – 80% of the dataset used for training purposes (includes labels).
- **📂 product_test.csv** – 20% of the dataset used for testing purposes (does not include labels).

## Preprocessing Steps
1. **Text Cleaning**
   - Removed special characters, numbers, and irrelevant content.
   - Standardized text by converting it to lowercase.

2. **Feature Engineering**
   - Applied TF-IDF Vectorization to convert text into numerical representations.
   - Employed word embeddings (e.g., Word2Vec) for enhanced feature representation.

3. **Category Mapping**
   The `product_category_name_english` column has been mapped to values between **1** and **9** for simplified classification. The mapping is as follows:

| Category Name | Mapped Value |
|---------------------------|-----------------|
| bed_bath_table             | 1               |
| health_beauty              | 2               |
| sports_leisure             | 3               |
| furniture_decor            | 4               |
| computers_accessories      | 5               |
| watches_gifts              | 6               |
| telephony                  | 7               |
| garden_tools               | 8               |
| auto                       | 9               |

4. **Dataset Splitting**
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
| Column Name | Description |
|--------------|--------------|
| Product Description | Detailed textual data describing the product features. |
| Category | Product category assigned to the item (already mapped to values 1-9). |
| Price | Product price information. |
| Summary | The summarized description generated for each product. |

## Usage
- Train your supervised learning model using `product_train.csv`.
- Evaluate your model's performance on `product_test.csv` and report accuracy and other metrics.

## Next Steps
- Experiment with various supervised learning models for optimal performance.
- Compare model performance using accuracy, R², F1 Score, or MSE as required.
