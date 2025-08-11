# Customer-Churn-Prediction-ML-Flask-Project

![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg) ![Flask](https://img.shields.io/badge/Flask-3.0-black.svg) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.5-orange.svg) ![Render](https://img.shields.io/badge/Render-Deployed-green.svg)

A complete end-to-end machine learning project that predicts customer churn. This application is built with a Python Flask backend, uses a trained Scikit-learn model, and is deployed on Render.

## 🚀 Live Demo

The application is deployed on Render and is publicly accessible.

*Live Link: [https://customer-churn-prediction-ml-flask.onrender.com](https://customer-churn-prediction-ml-flask.onrender.com)*

> *Note:* The application is hosted on Render's free tier, so it may take 30-60 seconds for the server to "wake up" on the first visit. Please be patient.

---

## 📸 Screenshot

 <img width="952" height="1080" alt="Screenshot 2025-08-12 021633" src="https://github.com/user-attachments/assets/fe199d88-7fd7-4a08-8d4c-3a32ce3e0761" />

---

## ✨ Features

- *Interactive Web Interface:* A user-friendly form built with HTML and Bootstrap to input customer data.
- *Real-time Predictions:* Submitting the form provides an instant prediction of whether a customer will "Churn" or "No Churn".
- *Probability Score:* In addition to the prediction, the model provides a confidence score (probability of churn).
- *End-to-End Pipeline:* Demonstrates the full ML lifecycle from data preprocessing and model training to deployment as a web service.

---

## 🛠 Technology Stack

- *Backend:* Python, Flask
- *Machine Learning:* Pandas, Scikit-learn
- *Frontend:* HTML, Bootstrap (via CDN)
- *Deployment:* Gunicorn, Render

---

## ⚙ How It Works

The prediction pipeline operates as follows:

1.  *User Input:* The user fills out the web form with 19 customer attributes.
2.  *Data Processing:* The Flask backend receives the form data and structures it into a Pandas DataFrame.
3.  *Encoding:* Categorical features (e.g., 'gender', 'Contract') are converted into numerical format using a pre-fitted encoder.pkl object.
4.  *Scaling:* Numerical features (e.g., 'tenure', 'MonthlyCharges') are normalized using a pre-fitted scaler.pkl object.
5.  *Prediction:* The fully processed data is fed into the trained machine learning model (best_model.pkl), which outputs the final prediction and probability.
6.  *Display Results:* The results are dynamically rendered on the web page.

---

## 📂 Project Structure


| File / Folder | Type | Purpose |
| :--- | :--- | :--- |
| 📁 templates/ | *Folder* | Contains all HTML templates for the user interface. |
| └── 📄 index.html | *HTML Template* | The main web page with the input form for users. |
| 📄 api.py | *Python Script* | The main Flask application that handles web requests and predictions. |
| 📄 requirements.txt | *Dependency File* | Lists all required Python packages for the project to run. |
| 📄 best_model.pkl| *ML Model* | The serialized, pre-trained machine learning model for making predictions. |
| 📄 encoder.pkl | *ML Artifact* | The fitted object for converting categorical text data into numbers. |
| 📄 scaler.pkl | *ML Artifact* | The fitted object for normalizing numerical data. |
| 📄 .gitignore | *Git Config File* | Specifies which files and folders Git should intentionally ignore. |
---
