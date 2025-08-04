# NSAP Eligibility Predictor using Machine Learning

A Flask-based machine learning application that predicts the most suitable NSAP welfare scheme (Old Age, Widow, Disability) based on user input.

## 🔧 Tech Stack
- Python, Flask, scikit-learn
- IBM Cloud Lite (Cloud Foundry deployment)
- Pandas, Joblib

## 🚀 API Usage
- **POST** `/predict`
- **Request Body:**
```json
{
  "age": 70,
  "income": 2000,
  "gender": "F",
  "is_disabled": 0,
  "is_widow": 1
}
```
- **Response:**
```json
{
  "predicted_scheme": "Indira Gandhi Widow Pension Scheme"
}
```

## 📦 Deployment
Deploy on IBM Cloud using:
```bash
ibmcloud login
ibmcloud target --cf
ibmcloud cf push
```
