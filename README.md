# Predicting Zodiac Signs Based on Personality Traits

## Overview
This project is my final portfolio project for the Codecademy Data Science and Machine Learning Career Path. The goal was to investigate whether it is possible to predict a person's zodiac sign based solely on their personality traits, using data from the OkCupid app. The underlying hypothesis—rooted in the belief that zodiac signs influence personality—was put to the test with a data-driven approach.

## Dataset
The dataset originates from OkCupid and contains anonymized user profiles with a wide range of features, including:
- **Demographics:** `age`, `ethnicity`, `sex`, `height`, `location`, `job`, `income`, `education`, `status`
- **Lifestyle Attributes:** `body_type`, `diet`, `drinks`, `drugs`, `smokes`, `pets`, `offspring`
- **Personality & Behavioral Data:** Multiple essay responses (`essay0` to `essay9`), `orientation`, `religion`, `sign`, `speaks`, `last_online`

## Technologies Used
- **Data Cleaning & Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn (Random Forest, KNN, Decision Tree, Logistic Regression)
- **Model Evaluation:** Accuracy, precision, recall, and f1-score metrics

## Methodology
1. **Data Cleaning:**  
   - Dropped rows with NaN values to avoid introducing bias from imputation.
   - Standardized feature labels and ensured consistency across the dataset.
   
2. **Exploratory Data Analysis (EDA):**  
   - Visualized the distribution of zodiac signs and other key features.
   - Investigated potential relationships between personality traits and zodiac signs.

3. **Feature Engineering:**  
   - Selected features with the best distribution for model training.
   - Applied one-hot encoding to categorical variables for use in machine learning models.

4. **Model Building & Evaluation:**  
   - Implemented four models: Logistic Regression, Decision Tree, KNN, and Random Forest.
   - Performed hyperparameter tuning using GridSearchCV for Random Forest and applied regularization for Logistic Regression.
   - Evaluated all models using metrics such as accuracy, precision, recall, and f1-score.
   - Despite Random Forest achieving the highest accuracy (~8.7%), its performance was no better than random guessing.

5. **Conclusion:**  
   The results indicate that, with this dataset, it is not possible to predict a person's zodiac sign based solely on their personality traits. Even after applying various modeling techniques and optimizations, the models consistently performed poorly, suggesting there is no meaningful correlation between the two.

6. **Future Work:**  
   - **NLP Analysis:** Train Natural Language Processing (NLP) models to analyze users' essay responses to extract deeper insights into personality.
   - **Advanced Feature Engineering:** Explore more sophisticated feature extraction and dimensionality reduction techniques.
   - **Alternative Models:** Experiment with other algorithms or ensemble methods to further probe the relationship between personality and zodiac signs.

## How to Run the Project
1. **Clone the Repository:**  
   ```bash
   git clone <repository_url>
