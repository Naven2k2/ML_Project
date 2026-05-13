# 🔮 TGNPDCL Energy Consumption Prediction System

An end-to-end Machine Learning + Streamlit web application that predicts electricity consumption units using infrastructure, load, and service-related features. The project uses a Random Forest Regressor model with feature engineering and is deployed using Hugging Face Spaces.

---

# 🚀 Live Demo

👉 https://huggingface.co/spaces/Naveen123hh/TGNPDCL_ENERGY_CONSUMPTION

---

# 📌 Project Overview

This project predicts electricity usage (Units Consumption) based on:

- Circle
- Division
- SubDivision
- Section
- Load
- Total Services
- Billed Services

The system uses Machine Learning techniques and feature engineering to improve prediction accuracy.

---

# 🧠 Machine Learning Workflow

## 🔹 Feature Engineering

```python
Load_per_Service = Load / TotServices
Billing_Ratio = BilledServices / TotServices
Log_Load = log(1 + Load)
```

## 🔹 Preprocessing

- Categorical Features → OneHotEncoder
- Numerical Features → Pass-through
- Combined using ColumnTransformer

## 🔹 Model Used

### RandomForestRegressor

| Hyperparameter | Value |
|---|---|
| n_estimators | 334 |
| max_depth | 21 |
| min_samples_split | 7 |
| min_samples_leaf | 1 |
| max_features | sqrt |

---

# 🛠️ Tech Stack

- Python 🐍
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Joblib
- Hugging Face Spaces

---

# 📁 Project Structure

```text
TGNPDCL_ENERGY_CONSUMPTION/
│
├── streamlit_app.py
├── model_training.py
├── rf_units_model.pkl
├── cleaned_data.xls
├── requirements.txt
└── README.md
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/TGNPDCL_ENERGY_CONSUMPTION.git
cd TGNPDCL_ENERGY_CONSUMPTION
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Application

```bash
streamlit run streamlit_app.py
```

---

# 🧪 Train the Model

```bash
python model_training.py
```

---

# 🖥️ App Inputs

- Circle
- Division
- SubDivision
- Section
- Load
- Total Services
- Billed Services

---

# 📈 Output

✅ Predicted Electricity Consumption Units

---

# 📊 Key Features

- 📥 Interactive Streamlit UI
- 🧠 Random Forest Regression Model
- ⚙️ Feature Engineering
- 🔄 Real-time Prediction
- 💾 Model Serialization using Joblib
- ☁️ Cloud Deployment on Hugging Face

---

# 📌 Future Improvements

- 📊 Add model evaluation metrics (R², RMSE)
- 📉 Add visualization dashboard
- 🤖 Integrate XGBoost / LightGBM
- 🌐 Deploy using AWS or Docker
- 📈 Add advanced analytics

---

# 👨‍💻 Author

## Naveen

Machine Learning & Data Science Enthusiast passionate about building AI-powered predictive systems and real-world ML applications.
