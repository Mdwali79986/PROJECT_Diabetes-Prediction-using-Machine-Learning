# 🩺 Diabetes Prediction using Support Vector Machine (SVM)

A machine learning project that predicts whether a person is diabetic or not based on diagnostic health measurements, using the **PIMA Indians Diabetes Dataset** and a **Support Vector Machine (SVM)** classifier.

---

## 📌 Project Overview

This project aims to build a binary classification model that can predict the likelihood of diabetes in a patient. It covers the full ML pipeline — from data loading and exploration to model training, evaluation, and a real-time predictive system.

---

## 📂 Dataset

- **Name:** PIMA Indians Diabetes Dataset
- **Source:** Originally from the National Institute of Diabetes and Digestive and Kidney Diseases
- **Records:** 768 patients (female, at least 21 years old of Pima Indian heritage)
- **Target Column:** `Outcome` — `0` = Non-Diabetic, `1` = Diabetic

### Features

| Feature | Description |
|---|---|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skinfold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body mass index |
| DiabetesPedigreeFunction | Diabetes pedigree function score |
| Age | Age in years |

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries:**
  - `numpy` — numerical operations
  - `pandas` — data loading and analysis
  - `scikit-learn` — preprocessing, model training, and evaluation

---

## 🔄 Project Workflow

```
1. Data Collection & Loading
        ↓
2. Exploratory Data Analysis (EDA)
        ↓
3. Data Standardization (StandardScaler)
        ↓
4. Train-Test Split (80% train / 20% test)
        ↓
5. Model Training (SVM — Linear Kernel)
        ↓
6. Model Evaluation (Accuracy Score)
        ↓
7. Predictive System (single-instance prediction)
```

---

## 📊 Model Details

- **Algorithm:** Support Vector Machine (SVM) with a linear kernel
- **Train-Test Split:** 80% training, 20% testing (stratified split, `random_state=2`)
- **Preprocessing:** Feature standardization using `StandardScaler`

---

## ✅ Results

| Dataset | Accuracy |
|---|---|
| Training Data | ~78–79% |
| Test Data | ~77–78% |

> *Exact values may vary slightly based on environment.*

---

## 💡 Sample Prediction

```python
input_data = (5, 166, 72, 19, 175, 25.8, 0.587, 51)
# Output: The person is diabetic
```

The input is reshaped, standardized using the same scaler fitted on training data, and passed to the trained SVM model for prediction.

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mdwali79986/PROJECT_Diabetes-Prediction-using-Machine-Learning.git
   cd PROJECT_Diabetes-Prediction-using-Machine-Learning
   ```

2. **Install dependencies**
   ```bash
   pip install numpy pandas scikit-learn
   ```

3. **Add the dataset**
   - Download `diabetes.csv` from [Kaggle – PIMA Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
   - Place it in the project directory

4. **Run the notebook**
   ```bash
   jupyter notebook Project_Diabetes_Prediction.ipynb
   ```

---

## 📁 Project Structure

```
diabetes-prediction/
│
├── Project_Diabetes_Prediction.ipynb   # Main notebook
├── diabetes.csv                        # Dataset (not included — add manually)
└── README.md                           # Project documentation
```

---

## 👤 Author

**Md Waliullah**
- 📧 mdwali79986@gmail.com
- 🔗 [LinkedIn](https://www.linkedin.com/in/md-wali-a5a82425b/)
- 💻 [GitHub](https://github.com/Mdwali79986)

---

## 📃 License

This project is open-source and available under the [MIT License](LICENSE).
