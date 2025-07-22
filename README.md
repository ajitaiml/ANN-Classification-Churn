# ANN-Classification-Churn
🔁 ANN-Based Customer Churn Classifier
A simple machine learning web application built with Flask, utilizing an Artificial Neural Network (ANN) to classify whether a customer is likely to churn. This project focuses on model training, evaluation, and frontend-backend integration to visualize predictions based on telecom customer data.



## 🧾 Project Overview

This project uses an **Artificial Neural Network (ANN)** to predict **customer churn** for a bank based on user features like credit score, geography, age, and more. It includes a user-friendly **Streamlit web app** for predictions.

---

🧠 Tech Stack
<table> <tr> <th>Category</th> <th>Tool</th> <th>Usage</th> </tr> <tr> <td><strong>Programming Language</strong></td> <td><img src="https://cdn.worldvectorlogo.com/logos/python-5.svg" alt="Python" width="30"/> <strong>Python</strong></td> <td>Base language for model building, preprocessing, and app logic</td> </tr> <tr> <td><strong>Modeling</strong></td> <td><img src="https://cdn.worldvectorlogo.com/logos/tensorflow-2.svg" alt="TensorFlow" width="30"/> <strong>TensorFlow</strong></td> <td>Deep learning library used to build the ANN model</td> </tr> <tr> <td><strong>Modeling</strong></td> <td><img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Keras_logo.svg" alt="Keras" width="30"/> <strong>Keras</strong></td> <td>High-level API to define and train the ANN model on top of TensorFlow</td> </tr> <tr> <td><strong>Web App</strong></td> <td><img src="https://streamlit.io/images/brand/streamlit-logo-primary-colormark-darktext.png" alt="Streamlit" width="30"/> <strong>Streamlit</strong></td> <td>Framework to build and deploy an interactive web app for predictions</td> </tr> <tr> <td><strong>Preprocessing</strong></td> <td><img src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" alt="Scikit-learn" width="30"/> <strong>Scikit-learn</strong></td> <td>Used for scaling, encoding, and preprocessing tabular data</td> </tr> </table>

---

🗂️ Project Structure  
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
