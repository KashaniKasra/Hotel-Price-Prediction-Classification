# Hotel Price Prediction and Classification

This machine learning project focuses on predicting hotel price categories based on various features such as hotel type, location, star rating, facilities, and user reviews. The goal is to use classification models to group hotels into distinct price brackets (e.g., low, medium, high) and help users or agencies understand pricing trends.

## Objectives

- Clean and preprocess real-world hotel dataset.
- Extract and encode meaningful features for modeling.
- Apply classification algorithms to predict price categories.
- Evaluate model performance and tune for better accuracy.

## Data Preprocessing

- Handled missing values (e.g., in 'star_rating' and 'review_score').
- Label encoding and one-hot encoding applied to categorical features like 'hotel_type' and 'location'.
- Normalized numerical features such as review count and distance from city center.

## Feature Engineering

- Created new features such as:
  - `is_luxury` based on amenities and star rating.
  - `review_per_star`: average review per star level.
- Removed outliers using IQR filtering on price-related fields.

## Models Used

- **Logistic Regression** – Baseline classifier
- **Random Forest Classifier** – Ensemble model for non-linear relationships
- **XGBoost** – High-performance gradient boosting
- **SVM** – For margin-based classification

All models were evaluated using:
- Accuracy
- Precision / Recall
- Confusion Matrix
- Cross-validation (k=5)

## Results

- Best accuracy achieved using Random Forest (85.3%)
- XGBoost slightly behind but provided better precision for high-price class
- SVM underperformed due to unbalanced class distribution

## Tools and Libraries

- Python (Jupyter Notebook)
- pandas, numpy, scikit-learn, xgboost
- seaborn, matplotlib for data visualization

## Future Work

- Try deep learning models (e.g., MLP)
- Integrate NLP for review sentiment analysis
- Add price regression to predict exact values

---

> Course: Artificial Intelligence – Spring 2025  
> University of Tehran | School of Electrical & Computer Engineering