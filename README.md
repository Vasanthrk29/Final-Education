# 🎯 Student Performance Prediction using Machine Learning

## 📌 Project Overview
This project aims to predict student performance based on various socio-economic and academic factors. Using the **Student Performance Dataset** from the UCI Machine Learning Repository, we preprocess the data, perform exploratory data analysis (EDA), and apply machine learning models to classify students as either **high-performing** or **low-performing** based on their final grade (G3).

## 📂 Dataset Information
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00320/student.zip)
- The dataset contains **1044 student records** with **33 features**, including:
  - **Demographic details** (age, address, family size, etc.)
  - **Parental education & job roles**
  - **Academic history (grades, absences, study time, etc.)**
  - **Social & behavioral aspects (going out frequency, alcohol consumption, etc.)**

## 🛠️ Data Preprocessing
- **Handled Missing Values**
- **Encoded Categorical Variables** (using Label Encoding & One-Hot Encoding)
- **Standardized Numerical Features** (using StandardScaler)
- **Discretized Target Variable (G3)** into **binary classes**:
  - `1` → High Performance (G3 ≥ 8)
  - `0` → Low Performance (G3 < 8)

## 📊 Exploratory Data Analysis (EDA)
✔️ Displayed dataset summary, missing values, and data types
✔️ Analyzed distribution of final grades (G3)
✔️ Visualized key trends using histograms & correlation heatmaps

## 🤖 Machine Learning Model
We experimented with multiple classifiers, and **Random Forest** performed the best:
- **Model Used**: `RandomForestClassifier(n_estimators=200, random_state=42)`
- **Train-Test Split**: 80-20 ratio
- **Evaluation Metrics**:
  - ✅ **Accuracy**: **96.17%**
  - ✅ **Confusion Matrix**:
    ```
    [[ 14   7]
     [  1 187]]
    ```

## 📌 How to Run the Project
1. **Clone the repository**
   ```bash
   git clone https://github.com/Vasanthrk29/Final-Education.git
   cd final_education
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Python script**
   ```bash
   python final_education.py
   ```

## 🚀 Future Enhancements
🔹 Implement Deep Learning models for better accuracy
🔹 Hyperparameter tuning to optimize the model
🔹 Deploy the model using Flask/Streamlit for real-time predictions

## 🏆 Contributors
👨‍💻 **Your Name** – [GitHub Profile](https://github.com/Vasanthrk29)

## 📜 License
This project is licensed under the **MIT License**. Feel free to use and modify!
