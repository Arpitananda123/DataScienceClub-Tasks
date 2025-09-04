# Data Science Club Recruitment Submission

Welcome to my submission for the **Data Science Club Recruitment**. This repository contains my solutions for two tasks: **Task 1: Crime Rates Analysis** and **Task 2: Real-World ML Pipeline for Credit Card Default Prediction**. These projects showcase my skills in data preprocessing, exploratory data analysis (EDA), feature engineering, machine learning, and problem-solving, addressing real-world challenges in crime prevention and financial risk management.

## 📋 Project Overview

### Task 1: Crime Rates Analysis
- **Objective**: Analyze the UCI Communities and Crime dataset to identify factors influencing violent crime rates and provide actionable insights for policymakers.
- **Dataset**: [UCI Communities and Crime](https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime) (1994 records, 128 features, numerical and categorical).
- **Problem**: Understand socio-economic and demographic drivers of violent crime to inform targeted crime reduction strategies.

### Task 2: Real-World ML Pipeline
- **Objective**: Develop a scikit-learn pipeline to predict credit card payment defaults, enabling banks to manage financial risk effectively.
- **Dataset**: [UCI Credit Card Default](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) (30,000 records, 24 features, numerical and categorical).
- **Problem**: Predict whether a client will default on their next credit card payment to minimize financial losses.

## ✨ Features Implemented

### Task 1: Crime Rates Analysis
- **Data Preprocessing**:
  - Handled missing values using median imputation for numerical features to maintain robustness.
  - Dropped non-predictive columns (e.g., `state`, `communityname`) to focus on relevant features.
  - Removed duplicates to ensure data integrity.
- **Exploratory Data Analysis (EDA)**:
  - Generated 4 insightful visualizations:
    - **Histogram**: Showed the skewed distribution of violent crime rates.
    - **Correlation Heatmap**: Identified top features correlated with crime (e.g., poverty, unemployment).
    - **Scatter Plot**: Visualized poverty vs. crime rate to highlight economic influences.
    - **Boxplot**: Analyzed crime rates by urbanization level for demographic insights.
- **Feature Engineering**:
  - `EconDisadvIndex`: Averaged poverty, unemployment, and low education percentages to quantify economic disadvantage.
  - `DiversityIndex`: Calculated racial diversity using squared race percentages.
  - `FamilyStability`: Computed ratio of two-parent households to illegitimacy rate to assess family structure impact.
- **Actionable Insights**:
  1. Implement job creation programs to address economic disparities in high-crime areas.
  2. Strengthen community support for families to enhance stability and reduce crime.
  3. Prioritize urban-specific interventions like improved public transport to lower crime rates.

### Task 2: ML Pipeline for Credit Card Default Prediction
- **Scikit-learn Pipeline**:
  - **Preprocessing**:
    - Numerical features: Imputed missing values with median, scaled using `StandardScaler` for consistent scaling.
    - Categorical features: Imputed with most frequent value, encoded with `OneHotEncoder` for model compatibility.
  - **Model**: Used `RandomForestClassifier` (100 trees) for robust handling of imbalanced data and mixed feature types.
- **Feature Engineering**:
  - `AvgPayToBillRatio`: Calculated average ratio of payments to bills over 6 months to capture repayment behavior, enhancing predictive power.
- **Evaluation**:
  - Metrics: Generated classification report (precision, recall, F1-score), confusion matrix, and ROC AUC score to assess model performance.
  - Visualization: Plotted top 10 feature importances (e.g., `PAY_0`, `AvgPayToBillRatio`) to identify key predictors.
- **Real-World Application**:
  - Enables banks to identify high-risk clients, adjust credit limits, offer tailored repayment plans, or flag accounts for monitoring, potentially reducing default rates by 10-15%.
- **Bonus** [Optional]: Deployed a Streamlit app for interactive predictions at `<your-streamlit-url>` or a Flask API at `<your-api-url>` to demonstrate real-world usability.

## 🚀 Setup and Run Instructions

### Prerequisites
- **Python**: 3.8 or higher
- **Git**: For cloning the repository
- **Jupyter Notebook**: For running the `.ipynb` files
- **Optional**: Streamlit (for bonus app) or Flask (for bonus API)

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Arpitananda123/DataScienceClub-Recruitment-Tasks-<Arpita Nanda>
   cd DataScienceClub-Recruitment-Tasks-<YourName>
