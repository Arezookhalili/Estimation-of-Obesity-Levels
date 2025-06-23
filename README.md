# 🧠 Classification of Obesity Levels Based on Eating Habits and Physical Condition

## 🔍 Project Summary

**Project Type:** Supervised Multi-Class Classification  
**Tools Used:** Python, Pandas, Scikit-learn, XGBoost, Random Forest, SHAP  
**Best Model Accuracy:** 96.1% (XGBoost)  
**Goal:** Predict individual obesity levels based on demographic, lifestyle, and behavioral features

---

## 🗂 Project Overview

This project applies machine learning techniques to predict obesity levels based on physical characteristics (e.g., age, gender, height, weight) and lifestyle habits (e.g., exercise, diet, water intake, tech usage, smoking).  
Dataset: [Estimation of Obesity Levels Based on Eating Habits and Physical Condition](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)

- 📊 **2111 records**
- ⚙️ **16 features**
- 🎯 **7 obesity classes**

---

## 🌐 Dataset Insights

- **Synthetic + real data**: 77% synthetic via SMOTE, 23% survey-based
- Balanced multi-class dataset
- Target variable: `Obesity_Level`  
  Classes:
  - 0: Insufficient Weight
  - 1: Normal Weight
  - 2: Overweight Level I
  - 3: Overweight Level II
  - 4: Obesity Type I
  - 5: Obesity Type II
  - 6: Obesity Type III

👉 See [data/README.md](data/README.md) for column descriptions.

---

## 💡 Key Results & Insights

- ✅ **XGBoost accuracy:** 96.1%
- ✅ Robust performance even when excluding `height` and `weight`
- ✅ Top features (via SHAP):
  - Age
  - Frequency of Vegetable Consumption
  - Gender
  - Water Intake
  - Tech Use
  - Physical Activity
  - Number of Meals
  - Family History

---

## 📊 Use Cases

| Sector | Application |
|--------|-------------|
| **Public Health** | Targeted education campaigns |
| **Healthcare** | Personalized risk screening & recommendations |
| **Insurance** | Dynamic health premiums based on predicted risk |

---

## 🔬 Methodology Summary

### A. Exploratory Data Analysis (EDA)

- Distribution plots (age, class, meals, etc.)
- Outlier detection & correlation matrix
- Box plots, bar charts, and scatter plots
- Key insights (e.g., more women classified as obese, low % walking/biking)

### B. Data Cleaning

- Removed duplicates and outliers
- Handled missing values
- One-hot encoded categorical variables
- Standardized numerical features

### C. Machine Learning & Modeling

- Models: Decision Tree, KNN, Random Forest, XGBoost
- Metrics: Accuracy, Precision, Recall, F1-score
- GridSearchCV & 5-fold cross-validation
- Model Comparison with and without height/weight

### D. Feature Engineering

- Feature importance via SHAP & Random Forest
- Eliminated low-impact and correlated variables
- Created reduced feature set for model simplification

### E. Results Overview

| Model Version | Accuracy |
|---------------|----------|
| XGBoost (all features) | 96.1% |
| Random Forest (all features) | 93.7% |
| XGBoost (excluding height/weight) | ~93% |
| XGBoost (top 8 features) | ~91% |

📷 [Model Comparison Image](https://github.com/user-attachments/assets/aa63819b-5b34-46d8-a177-13cf16565fc5)

---

## 🚀 Future Scope

- Fine-tune XGBoost on external datasets
- Test real-world deployment on unseen samples
- Explore explainability frameworks (e.g., LIME, SHAP UI)
- Build a simple risk score/recommendation engine for public health use

---

## 🧪 Team Contributions

| Task | Lead | Support |
|------|------|---------|
| EDA | Jyoti | Arezoo |
| Data Cleaning | Arezoo | Zekiye |
| Encoding & Scaling | Kathryn | — |
| ML Modeling | Zekiye | Jyoti |
| Feature Engineering | Zekiye | Arezoo |
| Reporting | Kathryn | All Members |

---

## 🎥 Presentations

| Team Member | GitHub | Video |
|-------------|--------|-------|
| **Arezoo Khalili** | [Arezoo Khalili](https://github.com/Arezookhalili) | [Watch](https://drive.google.com/file/d/1R9KJtClii35X0K13XacfvGpxG0r_dh9j/view?usp=drive_link) |
| **Jyoti Narang** | [drop2jyoti](https://github.com/drop2jyoti) | [Watch Folder](https://drive.google.com/drive/folders/1kZ9L8xZUXKYOCRIFD6hSeOCnnMrqTmZb) |
| **Kathryn Vozoris** | [KathrynVozoris](https://github.com/KathrynVozoris) | *Not Provided* |
| **Zekiye Erdem** | [zekiyerdem](https://github.com/zekiyerdem) | [Watch Folder](https://drive.google.com/drive/folders/1edbiriTnRMPIYdsnzrAsmYj4fHGTJP6n?usp=sharing) |

---

## 📁 Project Links

- 🗂 [GitHub Project Board](https://github.com/users/drop2jyoti/projects/2)
- 🖼 [Image Gallery](https://github.com/drop2jyoti/Estimation-of-Obesity-Levels/blob/main/reports/Images.md)
- 📓 [Jupyter Notebooks](notebooks)
- 📦 [requirements.txt](requirement.txt)

