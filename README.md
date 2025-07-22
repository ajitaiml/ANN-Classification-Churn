# ANN-Classification-Churn

This project uses an Artificial Neural Network (ANN) to predict **customer churn** based on banking customer data. It helps businesses identify customers likely to leave and take preventive action.

## 🧾 Project Overview

- **Goal**: Predict whether a customer will exit (churn) the bank.
- **Model**: ANN built using TensorFlow/Keras.
- **Accuracy**: Achieved ~85% on test data.
- **Interface**: Interactive prediction using a **Streamlit** app.

---

## 🧠 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- TensorFlow / Keras
- Streamlit
- Pickle (for model serialization)

---

## 🗂️ Files & Structure

```
├── Churn_Modelling.csv             # Dataset
├── app.py                          # Streamlit web app
├── experiments.ipynb               # Model training and evaluation
├── prediction.ipynb                # Predict using trained model
├── model.h5                        # Saved trained model
├── label_encoder_gender.pkl        # Encoder for 'Gender'
├── onehot_encoder_geo.pkl          # Encoder for 'Geography'
├── scaler.pkl                      # StandardScaler for features
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation
```

---

## 🔍 Dataset Summary

- **Source**: `Churn_Modelling.csv`
- **Rows**: 10,000 customers
- **Features**:
  - CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, etc.
- **Target**: `Exited` (1 = Churned, 0 = Stayed)

---

## 📊 Model Summary

- **Input**: 11 customer features after encoding/scaling
- **Architecture**:
  - Dense → ReLU
  - Dense → ReLU
  - Output → Sigmoid
- **Loss**: Binary Crossentropy
- **Optimizer**: Adam
- **Performance**: ~85% accuracy

---

## 🚀 How to Run the App

### 1. Clone the repository

```bash
git clone https://github.com/ajitaiml/ANN-Classification-Churn.git
cd ANN-Classification-Churn
```

### 2. Install required libraries

```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit app

```bash
streamlit run app.py
```

### 4. Open in Browser

Go to: `http://localhost:8501`

---

## 📌 Use Cases

- Banks and fintech companies for customer retention
- Subscription-based services (telecom, SaaS)
- Customer relationship management systems

---

## 📄 License

This project is licensed under the **GPL-3.0 License**.

---

## 🙋‍♂️ Author

**Ajit Singh**  
[GitHub](https://github.com/ajitaiml)
