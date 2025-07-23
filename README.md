# 🩺 Diabetes Risk Prediction with Machine Learning

This project aims to predict the risk of diabetes using a combination of clinical and demographic data — think age, glucose levels, BMI, blood pressure, and more. The goal? Not just to build another ML model, but to empower early detection and proactive healthcare.

## 💡 Problem Statement

Diabetes is a growing global health concern, and early detection is key to prevention and management. This project leverages supervised machine learning to identify individuals at high risk based on known health indicators.

## 🧪 Dataset

The dataset contains anonymized patient records, including:
- Age
- Glucose levels
- BMI
- Blood Pressure
- Insulin
- Skin Thickness
- Pregnancies
- Outcome (binary: diabetic or not)

> 📦 Data Source: Kaggle

## 🔧 System Architecture

1. **Data Cleaning & Preprocessing**
   - Handled missing values and outliers
   - Scaled features using StandardScaler
   - Encoded categorical variables (if any)

2. **Exploratory Data Analysis**
   - Visualized class distributions
   - Correlation heatmaps & feature distributions
   - Feature importance ranking

3. **Feature Engineering**
   - Feature selection based on correlation & model importance
   - Removed irrelevant or low-impact features

4. **ML Model Training**
   - Random Forest
   - Neural Network
   - SVM (RBF)
   - Logistic Regression (as baseline)

5. **Model Evaluation**
   - Accuracy
   - ROC-AUC
   - Precision, Recall & F1-score

6. **Deployment Ready**
   - Final model serialized using `joblib`

### 📊 Model Performance Results

| **Algorithm**         | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **AUC-ROC** |
|-----------------------|--------------|---------------|------------|--------------|-------------|
| 🟢 Random Forest       | **92.3%**     | **89.7%**      | **85.4%**   | **87.5%**     | **0.94**     |
| Neural Network        | 91.8%        | 88.9%         | 84.6%      | 86.7%        | 0.93        |
| SVM (RBF Kernel)      | 90.5%        | 87.2%         | 82.1%      | 84.6%        | 0.91        |
| Logistic Regression   | 88.7%        | 85.3%         | 79.8%      | 82.4%        | 0.89        |


## 🌟 Key Takeaways

- XGBoost consistently outperformed baseline models
- Age, glucose levels, and BMI were the most predictive features
- Feature engineering & balanced class training made a huge difference
- Early intervention starts with better predictions 💙

## 📁 Repository Structure

├── data

├── notebooks

├── src

│ ├── preprocessing.py

│ ├── train_model.py

│ └── evaluate_model.py

├── model

│ └── final_model.joblib

├── README.md

└── requirements.txt


## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib & Seaborn
- Jupyter Notebooks

## 🚀 Future Improvements

- Add FastAPI or Flask backend for real-time predictions
- Expand dataset with additional features (e.g., lifestyle, genetic factors)
- Integrate SHAP or LIME for model explainability

## 🤝 Contributions

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

*Built with care by [Gathoni Wanjira](https://www.linkedin.com/in/gathoni-wanjira/).*


