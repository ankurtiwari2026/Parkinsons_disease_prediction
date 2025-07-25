# 🧠 Parkinson's Disease Prediction using Machine Learning

![Brain Scan](https://cdn.pixabay.com/photo/2019/09/05/14/39/mri-4453115_1280.jpg)
*Helping detect Parkinson’s early through machine learning.*

---

## 📌 Project Overview

This project aims to **predict Parkinson’s Disease** using machine learning algorithms trained on vocal biomarker data. Parkinson’s Disease is a long-term degenerative disorder of the central nervous system that mainly affects motor function. By analyzing voice patterns and other clinical features, our model can predict whether a patient is likely to have Parkinson’s.

This tool can serve as an **assistive diagnostic system** for medical practitioners and researchers — especially in areas where access to neurologists or imaging tools is limited.

---

## 🎯 Objectives

- Predict Parkinson’s Disease with high accuracy using biomedical voice data.
- Build a lightweight, easy-to-use ML pipeline for real-world applications.
- Visualize important features contributing to prediction.
- Provide an optional user interface for live prediction.

---

## ⚙️ Technologies Used

| Tool         | Purpose                      |
|--------------|------------------------------|
| Python       | Core language for ML & logic |
| Scikit-learn | ML modeling and training     |
| Pandas       | Data preprocessing           |
| NumPy        | Numeric computation          |
| Seaborn      | Data visualization           |
| Matplotlib   | Graph plotting               |
| Streamlit    | Web app interface (optional) |
| Jupyter Lab  | Exploratory analysis         |

---

## 🧪 Dataset

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/parkinsons)
- **Dataset Size**: 195 rows × 23 features

### Key Features:

- `MDVP:Fo(Hz)`: Average vocal fundamental frequency  
- `Jitter`, `Shimmer`: Frequency and amplitude perturbations  
- `HNR`: Harmonic-to-noise ratio  
- `Spread1`, `Spread2`, `D2`, `PPE`: Measures of signal complexity  

---

## 📊 Exploratory Data Analysis

![EDA - Correlation Matrix](https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/Correlation_matrix.svg/640px-Correlation_matrix.svg.png)  
*Visualizing feature correlation to identify important biomarkers.*

We explored feature relationships, distributions, and outliers. Strong correlations were found between specific vocal metrics and Parkinson’s diagnosis.

---

## 🤖 Machine Learning Model

We experimented with multiple algorithms:

- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- XGBoost  

> ✅ **Best Performance**: SVM with ~94% accuracy after scaling and tuning.

### Evaluation Metrics:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

![Confusion Matrix](https://miro.medium.com/v2/resize:fit:700/format:webp/1*bkgRBD9eOUO7U1xWhC5nMA.png)  
*A sample confusion matrix from model evaluation.*

---

## 🔍 Feature Importance

We used model explainability tools like **SHAP** and built-in `feature_importances_` to visualize which features contribute most to predictions.

![Feature Importance](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/03/shap.png)  
*SHAP summary plot showcasing important features.*

---

## 💻 User Interface (Optional)

A simple UI built using **Streamlit** allows users to input feature values and receive instant predictions.

![Streamlit Logo](https://streamlit.io/images/brand/streamlit-logo-primary-colormark-darktext.png)  
*Live prediction app interface (demo concept).*

---

## 🚀 How to Run the Project

Follow the steps below to clone, install, and run the project:

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/Parkinsons_disease_prediction.git
cd Parkinsons_disease_prediction
