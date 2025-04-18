# Credit Card Fraud Detection

Detecting fraudulent transactions in credit card data using machine learning.

## Overview

This project focuses on identifying fraudulent credit card transactions using a dataset of transactions made by European cardholders in September 2013. Out of 284,807 transactions, only 492 are fraudulent — highlighting a major class imbalance (0.172%).

The project aims to develop a classification model that can accurately detect fraudulent transactions using effective data preprocessing, balancing techniques, and hyperparameter tuning.

## Objectives

- Perform exploratory data analysis (EDA) to understand the data and uncover insights.
- Preprocess data by handling missing values, duplicates, and outliers.
- Engineer features that improve the model's predictive power.
- Train multiple classification models and evaluate their performance.
- Apply data balancing techniques to address class imbalance.
- Optimize model performance with hyperparameter tuning using `RandomizedSearchCV`.

## Dataset

- **Source**: [Download Dataset](https://kh3-ls-storage.s3.us-east-1.amazonaws.com/DS%20Project%20Guide%20Data%20Set/creditcard.csv)
- **Total transactions**: 284,807
- **Fraudulent transactions**: 492 (~0.172%)
- **Time period**: Two days of transactions by European cardholders
- **Features**: Includes anonymized features (V1–V28), Time, Amount, and Class (target)

## Getting Started

### Prerequisites

Ensure you have Python 3.10.14 installed. Required libraries include:

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

### Installation

Clone the repository:

```bash
git clone https://github.com/Amra-Shaikh/FindDefault.git
cd FindDefault
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

Follow these steps to replicate the results:

1. Load the dataset (`creditcard.csv`).
2. Perform exploratory data analysis (EDA) to identify patterns.
3. Preprocess the dataset:
   - Remove duplicates
   - Handle missing values
   - Detect and treat outliers
4. Apply data balancing techniques (e.g., SMOTE or undersampling).
5. Train various classification models.
6. Evaluate models using appropriate metrics: precision, recall, F1-score, ROC-AUC.
7. Tune hyperparameters using `RandomizedSearchCV`.
8. Test the model on unseen data and assess generalization performance.

## Project Structure

```
FindDefault/
│
├── data/            # Contains the raw dataset (e.g., creditcard.csv)
├── models/          # Directory to save trained model files
├── notebook/        # Jupyter notebooks for EDA, preprocessing, modeling, etc.
├── visuals/         # Plots, charts, and visual outputs for analysis
├── requirements.txt # List of dependencies
├── README.md        # Project documentation
└── LICENSE          # Project license information
```

## Results

After preprocessing and hyperparameter tuning, the selected model generalized well on unseen data, improving:

- Precision  
- Recall  
- F1-score  
- ROC-AUC  

Hyperparameter tuning using `RandomizedSearchCV` significantly enhanced the model's ability to detect fraud more accurately while minimizing false positives.

## Future Work

- Explore advanced models such as XGBoost, LightGBM, or deep learning architectures.
- Incorporate additional data sources such as user behavior or location data.
- Implement automated hyperparameter tuning using libraries like Optuna or Hyperopt.
- Deploy the model using a REST API for real-time fraud detection.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository  
2. Create a new branch  
3. Commit your changes  
4. Open a pull request  

For major changes, please open an issue first to discuss the proposed updates.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Dataset provided by: [Credit Card Fraud Detection Dataset](https://kh3-ls-storage.s3.us-east-1.amazonaws.com/DS%20Project%20Guide%20Data%20Set/creditcard.csv)
- Thanks to the open-source community and contributors for tools and resources.

## Tech Stack

- Python  
- Jupyter Notebook  
- Scikit-learn  
- Matplotlib  
- Seaborn  

## Maintainer

**Amra-Shaikh**  
GitHub: (https://github.com/Amra-Shaikh)
