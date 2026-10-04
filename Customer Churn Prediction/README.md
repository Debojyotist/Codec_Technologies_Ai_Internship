# 📉 Customer Churn Prediction App

A machine learning-powered web application built with **Streamlit** that predicts whether a customer is likely to churn based on their demographic information, account tenure, and monthly charges.

---

## 🚀 Live Demo
*https://churn-prediction-app-dst.streamlit.app/*

---

## 🛠️ Tech Stack & Libraries
* **Python** (Core programming language)
* **Streamlit** (Interactive web framework for ML apps)
* **Scikit-Learn** (Machine learning model and data scaling)
* **Joblib** (Model serialization and loading)
* **NumPy** (Numerical operations)

---

## 📂 Project Structure
```text
├── CCP.ipynb               # Jupyter Notebook for exploratory data analysis and model training
├── README.md               # Project documentation
├── app.py                  # Main Streamlit application script
├── customer_churn_data.csv # Raw dataset used for the machine learning model
├── model.pkl               # Trained machine learning model
├── requirements.txt        # Python package dependencies
└── scaler.pkl              # Fitted StandardScaler for input normalization
```

---

## 🧠 Input Features & Processing
The application takes the following user inputs and processes them before running predictions:
1. **Age**: Integer value ranging from 10 to 100 years.
2. **Gender**: Selected as `Male` or `Female` (Encoded automatically: `Female` = 1, `Male` = 0).
3. **Tenure**: Integer value representing months with the company (0 to 130 months).
4. **Monthly Charges**: Floating-point value representing monthly billing amount ($30 to $150).

> **Note:** The input vector `[Age, Gender, Tenure, MonthlyCharges]` is transformed using the pre-trained `scaler.pkl` to match the training distribution before being passed to `model.pkl`.

---

## ⚙️ Local Installation & Setup

Follow these steps to run the project locally on your machine:

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies
Make sure you have Python installed, then install the required packages:
```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit App
```bash
streamlit run app.py
```

---

## 📦 Deployment on Streamlit Community Cloud
1. Push your code, `model.pkl`, `scaler.pkl`, `app.py`, and `requirements.txt` to a public GitHub repository.
2. Go to [Streamlit Community Cloud](https://share.streamlit.io/).
3. Click **New app**, select your repository, branch, and main file path (`app.py`).
4. Click **Deploy**!

---

## 👤 Author
**Debojyoti Sinha Thakur**  
*B.Sc. Computer Science and Data Analytics — IIT Patna*
