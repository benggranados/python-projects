# Comparative Analysis of Machine Learning Models for American Option Pricing

This project evaluates and compares three machine learning models—Feed-Forward Neural Networks, Gradient Boosting, and XGBoost—for pricing American Call Options using synthetic data generated from the **Heston stochastic volatility model**.

## 📊 Project Summary
We analyze model performance on three datasets of increasing size (2K, 50K, 250K) to explore how each algorithm scales in terms of accuracy and computational efficiency. The models are tuned via GridSearch and evaluated using a custom trade-off metric (accuracy vs. time).

## 🔧 Tools & Libraries
- Python  
- NumPy, Pandas, Scikit-learn  
- XGBoost  
- Keras / TensorFlow (for neural networks)  
- Matplotlib / Seaborn  

## 🧠 Models Compared
- **Feed-Forward Neural Network**: High accuracy on large datasets, slower to train
- **Gradient Boosting**: Good balance of accuracy and speed
- **XGBoost**: Fastest and most accurate on small datasets, best trade-off overall

## 📈 Evaluation Metrics
- **Root Mean Squared Error (RMSE)**
- **Prediction Time (in seconds)**
- **Custom Trade-off Metric**: Penalizes both high error and slow runtime

## 📂 Files
- `Model_Comparison.ipynb` – Full notebook with data generation, model training, and evaluation
- `Comparative Analysis of Deep Learning and Ensemble Models...pdf` – Final report detailing methodology and findings

## 📌 Key Findings
- **XGBoost** performed best overall in speed-accuracy trade-off, especially on small datasets.
- **Neural Networks** achieved top accuracy on large datasets but at higher computational cost.
- The choice of model depends on whether speed or precision is more critical.

## 📎 Author
Ben Granados
