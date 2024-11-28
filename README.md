# Telco-Customer-Churn
## Overview
This project aims to predict customer churn in the telecommunications industry using advanced ensemble learning techniques and implement personalized retention strategies based on these predictions. The project emphasizes model explainability, providing clear insights into the factors driving customer churn predictions.

## Features
- **Churn Prediction:** Predicts which customers are at risk of leaving using ensemble learning models.
- **Cost-Sensitive Learning:** Models take into account the financial implications of churn, prioritizing high-cost churns.
- **Model Explainability:** Utilizes LIME and Counterfactual Explanations to provide transparency into model predictions.
- **Personalized Retention Strategies:** Implements customized interventions to reduce churn based on predictive insights.
- **Interactive Streamlit Application:** A user-friendly interface to interact with the model, visualize predictions, and understand the rationale behind them.

## Data
This project uses the **Telco Customer Churn dataset** from Kaggle.

## Modeling Approach

### Ensemble Learning Models:
- **Random Forest**
- **AdaBoost**
- **Stacking Classifier**

These models were selected for their robustness and ability to handle complex patterns in the data. Hyperparameter tuning was performed using **Random Search** to optimize model performance.

### Cost-Sensitive Learning:
A cost-sensitive approach was applied to minimize the financial impact of churn, ensuring that predictions prioritize high-risk customers who contribute significantly to revenue.

### Explainability

- **LIME (Local Interpretable Model-Agnostic Explanations):**
  LIME is used to explain individual model predictions, highlighting which features contribute most to the churn prediction for each customer.
  
- **Counterfactual Explanations:**
  Counterfactual explanations show how minimal changes in customer features could alter the churn prediction, providing actionable insights for retention strategies.

## Results
- **Accuracy:** The Stacking Classifier achieved an accuracy of **88.83%**.
- **AUC Score:** The model attained an **AUC score of 0.88**.
- **Churn Reduction:** Implemented strategies based on model predictions resulted in a **15% reduction in churn rates**.

## Installation
1. Clone the repository:
   
```bash
git clone https://github.com/AnshikaaSharmaa/Telco-Customer-Churn.git
```

2.  Navigate to the project directory:
   
```bash
cd Telco-Churn-Prediction
```

3. Install the required dependencies
```bash
pip install -r requirements.txt
```
## Streamlit Application

The project includes a Streamlit application that allows users to interact with the model predictions and visualize the explanations.

### To run the Streamlit app:

1. Navigate to the `streamlit_app` folder:

   ```bash
   cd streamlit_app
   ```
2. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

The app will be accessible at ```https://telco-churn-prediction.streamlit.app/.```

