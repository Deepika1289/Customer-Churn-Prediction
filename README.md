# Customer Churn Prediction

A machine learning project to predict customer churn using data analysis, visualizations, and predictive modeling techniques.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Key Features](#key-features)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Performance](#model-performance)
- [Predictions](#predictions)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results & Visualizations](#results--visualizations)
- [Contributing](#contributing)

## Overview

This project aims to predict which customers are likely to churn (leave) from a business using machine learning algorithms. Early identification of at-risk customers can help organizations implement retention strategies and reduce revenue loss.

## Project Description

Customer churn prediction is a critical business problem. This project implements a complete machine learning pipeline including:
- **Data Preprocessing**: Cleaning, encoding, and scaling data
- **Exploratory Data Analysis (EDA)**: Understanding customer behavior patterns
- **Feature Engineering**: Creating meaningful features for model training
- **Model Development**: Building and training multiple ML algorithms
- **Model Evaluation**: Assessing model performance using various metrics
- **Predictions**: Making churn predictions on new customer data

## Dataset

The dataset contains customer information including:
- **Demographic Data**: Age, gender, location
- **Account Information**: Tenure, contract type, monthly charges
- **Service Usage**: Internet service, phone service, streaming services
- **Target Variable**: Churn status (Yes/No)

**Dataset Size**: [Specify number of records and features]
**Time Period**: [Specify timeframe if applicable]

## Key Features

### Data Analysis & Visualizations

- **Churn Distribution**: Pie charts and bar plots showing churn vs. non-churn customers
- **Tenure Analysis**: Distribution of customer tenure and its relation to churn
- **Monthly Charges**: Visualization of billing patterns among churned vs. retained customers
- **Service Usage Patterns**: Analysis of various service subscriptions
- **Contract Type Impact**: How different contract types affect churn rates
- **Demographic Analysis**: Gender, location, and age-based churn insights
- **Correlation Heatmap**: Feature relationships and their impact on churn

### Exploratory Data Analysis (EDA)

The project includes comprehensive visualizations:
- Histograms for continuous variables
- Box plots for outlier detection
- Scatter plots for variable relationships
- Categorical distribution plots
- Correlation matrices
- Customer segment analysis

## Model Performance

### Models Implemented

1. **Logistic Regression** - Baseline model for binary classification
2. **Decision Tree Classifier** - Tree-based approach for interpretability
3. **Random Forest Classifier** - Ensemble method for robust predictions
4. **Gradient Boosting** - Advanced boosting technique
5. **Support Vector Machine (SVM)** - Kernel-based classification

### Performance Metrics

- **Accuracy**: Overall correctness of predictions
- **Precision**: Accuracy of positive predictions
- **Recall**: Ability to identify all churners
- **F1-Score**: Balance between precision and recall
- **ROC-AUC Score**: Model discrimination ability
- **Confusion Matrix**: Breakdown of predictions vs. actuals

### Best Model Results

[Models are trained and evaluated on the dataset. Results show performance comparisons.]

- Model with highest accuracy achieves **[X%]** accuracy
- Best F1-Score: **[X]**
- AUC-ROC Score: **[X]**

## Predictions

### Prediction Output

The model generates predictions for:
- **Probability of Churn**: Likelihood score (0-1) for each customer
- **Churn Classification**: Binary prediction (Yes/No)
- **Risk Segmentation**: Customers segmented into risk categories:
  - High Risk: Probability > 0.7
  - Medium Risk: Probability 0.3-0.7
  - Low Risk: Probability < 0.3

### Business Insights

- **High-Risk Customers**: Targeted retention campaigns
- **Churn Drivers**: Key factors influencing customer departure
- **Actionable Recommendations**: Steps to reduce churn rate

## Technologies Used

- **Python 3.x** - Programming language
- **Jupyter Notebook** - Interactive development environment
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Scikit-learn** - Machine learning algorithms
- **Matplotlib** - Static visualizations
- **Seaborn** - Statistical data visualization
- **Plotly** - Interactive visualizations (optional)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Deepika1289/Customer-Churn-Prediction.git
   cd Customer-Churn-Prediction
   ```

2. **Create a virtual environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Open Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

2. **Run the analysis notebooks**:
   - `01_Data_Preprocessing.ipynb` - Data cleaning and preparation
   - `02_EDA.ipynb` - Exploratory Data Analysis with visualizations
   - `03_Feature_Engineering.ipynb` - Feature creation and selection
   - `04_Model_Training.ipynb` - Model development and comparison
   - `05_Predictions.ipynb` - Making predictions on new data

3. **Review visualizations and results** at each step

## Results & Visualizations

### Key Visualizations Generated

1. **Churn Distribution Chart** - Overall churn percentage
2. **Feature Importance Plot** - Top factors driving churn
3. **ROC Curve** - Model performance visualization
4. **Confusion Matrix Heatmap** - Prediction breakdown
5. **Customer Tenure vs. Churn** - Long-term customer behavior
6. **Monthly Charges Distribution** - Pricing impact on churn
7. **Service Category Analysis** - Which services retain customers best
8. **Model Comparison Chart** - Performance across all models

### Key Findings

- [Insert main insights about customer churn patterns]
- [Key factors influencing customer retention]
- [Recommendations for reducing churn]

## Contributing

Contributions are welcome! Please feel free to:
- Report bugs or issues
- Suggest improvements
- Add new features or models
- Improve documentation

To contribute:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes and commit them
4. Push to the branch and create a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

---

**Author**: Deepika1289

**Last Updated**: May 2026

For questions or suggestions, please open an issue or contact the repository owner.
