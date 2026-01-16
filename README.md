**🧠 AI-Assisted Fraud Risk Prioritization for Digital Banking

📌 **Project Overview**
Banks process millions of digital transactions daily, but fraud investigation teams can only manually review a limited number of transactions due to time and cost constraints. Reviewing transactions randomly leads to very low fraud detection rates.

This project builds an AI-assisted decision support system that:

  1. Predicts fraud probability for each transaction using machine learning
  2. Ranks transactions by risk
  3. Selects the highest-risk transactions for investigation under limited capacity

The goal is not only prediction, but business-driven prioritization and operational optimization.

**🎯 Business Objective**
Given a daily review capacity of 100 transactions:

   1. Maximize number of fraud cases detected
   2. Improve investigation efficiency
   3. Reduce financial losses

This transforms fraud detection into a resource optimization problem, combining:

  1. Data analytics
  2. Artificial intelligence
  3. Operations research principles

📊 Dataset Description

**Dataset**: Credit Card Fraud Dataset (European cardholders)

  1. Total transactions: ~284,000
  2. Fraud cases: ~0.17% (highly imbalanced, realistic banking scenario)

**Features**:
  
  1. Time – Seconds elapsed between transactions
  2. Amount – Transaction amount
  3. V1–V28 – Anonymized transaction behavior features
  4. Class – Target variable (0 = Normal, 1 = Fraud)

Dataset source: https://drive.google.com/file/d/14D3Ro7xSQOPyt6acIE8G0RigeiSkgG-W/view 

**🧩 Methodology**

Step 1: Exploratory Analysis

  1. Compared average transaction amount for fraud vs normal transactions
  2. Observed higher average amount for fraudulent transactions

Step 2: Data Preparation

  1. Separated features and target variable
  2. Split data into:
       a. 70% Training
       b. 30% Testing

Step 3: AI Model Training

  1. Trained Logistic Regression classifier
  2. Model learns patterns that differentiate fraud from normal behavior

Step 4: Risk Scoring

  1. Predicted fraud probability (0 to 1) for each transaction
  2. Probability used as continuous risk score

Step 5: Risk-Based Prioritization

  1. Sorted transactions by predicted fraud probability
  2. Selected top 100 highest-risk transactions

Step 6: Business Evaluation

  1. Compared two strategies:
      a. AI-based prioritization
      b. Random transaction selection

📈 Results & Business Impact
Strategy	                 Fraud Detected in 100 Reviews
AI Prioritization               	94 fraud cases
Random Selection	                 0 fraud cases

**You can also run this notebook on Google Colab**: https://colab.research.google.com/drive/1cLgNPtCzRrSRmma1zSMhyve9_foZJjCw

**Key Insights:**

   1. Fraud transactions have higher average amounts than normal transactions
   2. AI-generated risk scores effectively rank true fraud cases at the top
   3. Prioritization dramatically improves investigator productivity

This demonstrates how AI can be used not just for prediction, but for decision-making under operational constraints.

🧠 Tools & Technologies

1. Python
2. Pandas
3. Scikit-learn
4. Matplotlib
5. Google Colab

📌 Why This Project Matters

This project reflects real-world challenges faced by:

 1. Banks
 2. Fintech companies
 3. Risk analytics teams

