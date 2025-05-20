# Comparative Analysis of Deep Learning and Ensembled Models for American Call Option Pricing

This project investigates the effectiveness of various machine learning models — including deep neural networks and ensemble methods — in pricing American call options. The analysis focuses on understanding how model performance varies across datasets of different sizes and characteristics.

## 📘 Project Objective

The aim was to evaluate how deep learning compares to classical ensemble models like Random Forests and Gradient Boosting in the context of financial derivatives pricing, specifically American call options where early exercise makes valuation more complex.

## 🧠 Models Compared

- **Deep Neural Networks (DNN)**
- **Random Forest Regressors**
- **Gradient Boosting Machines (XGBoost)**
- **Longstaff-Schwartz Method (baseline)**

## 🔍 Methodology

- **Data Simulation:**  
  Synthetic datasets were generated using Monte Carlo simulation for American call options under various underlying asset paths.

- **Model Training:**  
  Each model was trained on multiple datasets with varying sample sizes to study scalability and generalization.

- **Evaluation Metrics:**  
  - Mean Squared Error (MSE)  
  - R² Score  
  - Pricing Bias vs. Benchmark

- **Validation:**  
  Used k-fold cross-validation and visual diagnostics to ensure robustness of model comparison.

## 🧰 Tools & Libraries

- Python (NumPy, Pandas, Scikit-learn, XGBoost, TensorFlow/Keras)
- Matplotlib / Seaborn for visualization
- Jupyter Notebooks for experimentation

## 📈 Key Findings

- Deep neural networks outperformed ensemble models on large datasets but struggled with smaller sample sizes.
- Ensemble methods like Random Forests offered more stable performance with limited data.
- The Longstaff-Schwartz method still served as a strong baseline for smaller and mid-sized datasets.
