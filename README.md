# Income Classification Project

This project focuses on predicting whether an individual's income exceeds $50K/year based on census data. The project follows a complete machine learning pipeline from data preprocessing to model evaluation.

## Dataset

The dataset contains demographic and employment-related features including:
- **Demographics**: age, sex, race, native-country
- **Education**: education level, education number
- **Employment**: workclass, occupation, hours-per-week
- **Financial**: capital-gain, capital-loss
- **Personal**: marital-status, relationship
- **Target**: income (binary: >50K or <=50K)

## Project Structure

- `income_classification.py`: Main Python script containing the complete data analysis and modeling pipeline
- `requirements.txt`: Dependencies required to run the project
- `README.md`: This file

## Features

### Data Preprocessing
- Handles missing values (represented as '?' in the original data)
- Cleans and standardizes column names and values
- Performs feature engineering including:
  - Creating binary 'is_married' feature
  - Combining education and occupation features
  - Handling categorical variables through encoding

### Exploratory Data Analysis (EDA)
- Visualizations of feature distributions
- Analysis of relationships between features and target variable
- Identification of class imbalance

### Modeling
Multiple machine learning models are implemented and compared:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- AdaBoost
- SVM
- Voting Classifier

### Model Evaluation
- Hyperparameter tuning using GridSearchCV
- Handling class imbalance using SMOTE
- Performance metrics including:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC

## Results

The Gradient Boosting model achieved the best performance with:
- F1-score: 0.9118
- Balanced performance across precision and recall

## Getting Started

### Prerequisites
- Python 3.6+
- Required Python packages (see `requirements.txt`)

### Installation
1. Clone the repository
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the analysis:
   ```
   python income_classification.py
   ```

## Dependencies
- pandas
- numpy
- scikit-learn
- imbalanced-learn
- matplotlib
- seaborn

## Contributing

Feel free to submit issues and enhancement requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
