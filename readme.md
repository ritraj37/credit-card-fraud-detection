# 🚨 Credit Card Fraud Detection System

An intelligent web-based application that detects fraudulent transactions using **Machine Learning + Rule-Based Logic**.

---

## 📌 Project Overview

This project is designed to identify suspicious or fraudulent credit card transactions based on transaction details such as amount, location, time, and user behavior.

The system combines:

* 🤖 Machine Learning Model (LightGBM)
* ⚙️ Rule-Based Detection (High amount, odd timing, location anomaly)
* 🌐 Interactive Web App (Streamlit)

---

## 🚀 Features

* 🔍 Detects fraudulent transactions in real-time
* 💰 High-value transaction monitoring (> ₹7,00,000)
* 🌙 Suspicious time detection (0–4 AM, 11 PM)
* 📍 Location anomaly detection using distance
* 📊 Interactive UI built with Streamlit
* ⚡ Fast predictions using trained ML model

---

## 🛠️ Tech Stack

* **Python**
* **Pandas, NumPy**
* **Scikit-learn**
* **LightGBM**
* **Streamlit**
* **Geopy (for distance calculation)**

---

## 📂 Project Structure

```
PYTHON/
│
├── models/
│   ├── fraud_detection_model.jb
│   └── encoders_dict.jb
│
├── app.py
├── dataset.csv
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/fraud-detection-system.git
cd fraud-detection-system
```

### 2️⃣ Create virtual environment

```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

## 🧠 How It Works

1. User enters transaction details
2. Data is preprocessed and encoded
3. Distance between user and merchant is calculated
4. ML model predicts fraud probability
5. Rule-based checks override model for critical cases

---

## ⚠️ Fraud Detection Rules

* 🚨 Amount > ₹7,00,000 → Direct Fraud
* ⚠️ Amount > ₹5,00,000 → High Risk
* 🌙 Transactions at night → Suspicious
* 📍 Large distance → Possible fraud

---

## 📈 Future Improvements

* Add fraud probability score (%)
* Improve model accuracy with more data
* Add map-based visualization
* Deploy on cloud (Streamlit / Render)
* Integrate real-time payment APIs

---

## 👨‍💻 Author

**Ritu Raj**
MCA Student | Data Analyst | ML Enthusiast

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and share it!
