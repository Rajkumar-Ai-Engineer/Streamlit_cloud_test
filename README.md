```markdown
# Customer Churn Prediction Web App

An end-to-end Machine Learning web application deployed using Streamlit to predict bank customer churn. The project utilizes a trained deep learning / neural network model (`model.h5`) along with preprocessing pipelines for categorical encoding and feature scaling.

---

## 📌 Project Overview

Customer churn occurs when customers stop doing business with a company. This application predicts whether a bank customer is likely to churn based on demographic and banking behavior factors such as credit score, geography, gender, age, tenure, balance, number of products, credit card status, active membership, and estimated salary.

---

## 📁 Repository Structure

```text
├── logs/fit/                    # TensorBoard / training log files
├── Churn_Modelling.csv          # Dataset used for training and validation
├── data_transformation.ipynb    # Data exploration, preprocessing, and model training
├── app.py                       # Streamlit web application script
├── model.h5                     # Trained Keras/TensorFlow model
├── label_encoder_gender.pkl     # Label encoder for the 'Gender' feature
├── onehotEncoder.pkl            # One-hot encoder for categorical features (e.g., Geography)
├── scaler.pkl                   # StandardScaler object for feature normalization
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation

```

---

## ⚙️ Tech Stack

* **Frontend / Deployment:** [Streamlit](https://streamlit.io/)
* **Modeling:** TensorFlow / Keras
* **Data Preprocessing & Analysis:** Scikit-Learn, Pandas, NumPy
* **Environment Management:** Python

---

## 🚀 Getting Started

### 1. Prerequisites

Make sure you have Python 3.8+ installed on your system.

### 2. Clone the Repository

```bash
git clone [https://github.com/Rajkumar-Ai-Engineer/Streamlit_cloud_test.git](https://github.com/Rajkumar-Ai-Engineer/Streamlit_cloud_test.git)
cd Streamlit_cloud_test

```

### 3. Set Up a Virtual Environment

```bash
# On macOS/Linux
python3 -m venv venv
source venv/bin/activate

# On Windows
python -m venv venv
venv\Scripts\activate

```

### 4. Install Dependencies

```bash
pip install -r requirements.txt

```

### 5. Run the Application

Launch the Streamlit app locally:

```bash
streamlit run app.py

```

Open your browser and navigate to `http://localhost:8501` to use the application.

---

## 🧪 Model & Preprocessing Workflow

1. **Data Preprocessing:** Handled in `data_transformation.ipynb`, using:
* `label_encoder_gender.pkl` to encode gender attributes.
* `onehotEncoder.pkl` for multi-category features like geography.
* `scaler.pkl` to scale numerical features to standard distributions.


2. **Inference:** In `app.py`, user input is collected via interactive UI widgets, transformed using the pre-fitted pickle objects, and passed to `model.h5` to output a churn probability score.

---

## 📄 License

This project is open-source and available under the MIT License.

```

```
