# ANN-Classification-Churn

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
</p>

## 🧾 Project Overview

This project uses an **Artificial Neural Network (ANN)** to predict **customer churn** for a bank based on user features like credit score, geography, age, and more. It includes a user-friendly **Streamlit web app** for predictions.

---

## 🧠 Tech Stack

- 🐍 **Python**
- 🧪 **Scikit-learn**
- 🔶 **TensorFlow / Keras**
- 📊 **Pandas, NumPy**
- 🌐 **Streamlit** (Web App)
- 🧬 **Pickle** (Model & Encoder Storage)

---

## 🗂️ Project Structure

```
├── Churn_Modelling.csv             # Dataset
├── app.py                          # Streamlit web app
├── experiments.ipynb               # Model training and evaluation
├── prediction.ipynb                # Predict using trained model
├── model.h5                        # Trained ANN model
├── label_encoder_gender.pkl        # Label encoder (Gender)
├── onehot_encoder_geo.pkl          # One-hot encoder (Geography)
├── scaler.pkl                      # Scaler for numeric features
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation
```

---

## 📊 Dataset Summary

- **Source**: `Churn_Modelling.csv`
- **Rows**: 10,000 customer records
- **Features**:
  - CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, etc.
- **Target**: `Exited` (1 = churned, 0 = retained)

---

## 🧮 Model Architecture

- Input Layer → Dense (ReLU)
- Hidden Layer → Dense (ReLU)
- Output Layer → Dense (Sigmoid)
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Accuracy**: ~85% on test set

---

## 🚀 Running the Streamlit App

### 🔧 1. Clone the repository

```bash
git clone https://github.com/ajitaiml/ANN-Classification-Churn.git
cd ANN-Classification-Churn
```

### 📦 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 🖥️ 3. Launch the app

```bash
streamlit run app.py
```

Then open `http://localhost:8501` in your browser.

---

## 🎯 Use Cases

- 💳 Customer Retention for Banks and Financial Institutions
- 📞 Telecom Subscriber Management
- 💼 Subscription-based Business Analysis

---

## 📄 License

This project is licensed under the **GPL-3.0 License**.

---

## 👤 Author

**Ajit Singh**  
🔗 [GitHub](https://github.com/ajitaiml) | 💼 B.Tech AI & Data Science  
