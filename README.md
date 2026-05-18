# Laptop Price Prediction Project

## Overview

This project is a Machine Learning-based Laptop Price Prediction System that predicts the estimated price of a laptop based on its specifications such as brand, processor, RAM, storage, GPU, operating system, screen size, and other hardware features.

The project uses a trained ML model saved as `laptopmodel.pkl` to generate predictions.

---

# Features

* Predict laptop prices using machine learning
* Data preprocessing and feature engineering
* Model training and evaluation
* Saved trained model using Pickle (`.pkl`)
* User-friendly prediction workflow
* Scalable for deployment with Flask/Streamlit

---

# Tech Stack

* **Programming Language:** Python
* **Libraries Used:**

  * Pandas
  * NumPy
  * Scikit-learn
  * Pickle
  * Matplotlib / Seaborn (optional for visualization)
* **Model Type:** Regression Model

---

# Project Structure

```bash
Laptop-Price-Prediction/
│
├── data/
│   └── laptop_data.csv
│
├── notebooks/
│   └── model_training.ipynb
│
├── models/
│   └── laptopmodel.pkl
│
├── app.py
├── requirements.txt
├── README.md
└── assets/
```

---

# Dataset Information

The dataset contains laptop specifications such as:

* Brand
* Processor Type
* RAM Size
* Storage Type
* SSD/HDD Capacity
* GPU
* Operating System
* Screen Size
* Weight
* Touchscreen Availability
* IPS Display
* Resolution
* Price

The target variable is:

```python
Price
```

---

# Machine Learning Workflow

## 1. Data Collection

Collected laptop specification data from publicly available sources.

## 2. Data Cleaning

* Removed null values
* Handled duplicates
* Converted categorical variables
* Formatted numerical values

## 3. Feature Engineering

* Extracted processor generation
* Encoded categorical variables
* Converted memory sizes
* Created useful derived features

## 4. Model Training

Different regression algorithms can be tested:

* Linear Regression
* Random Forest Regressor
* Decision Tree Regressor
* XGBoost Regressor

Final trained model is stored as:

```bash
laptopmodel.pkl
```

---

# Model Evaluation

Common evaluation metrics used:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* RMSE (Root Mean Squared Error)
* R² Score

Example:

```python
R2 Score: 0.89
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/your-username/laptop-price-prediction.git
cd laptop-price-prediction
```

## Create Virtual Environment

```bash
python -m venv venv
```

Activate environment:

### Windows

```bash
venv\Scripts\activate
```

### Linux/Mac

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

Example `requirements.txt`:

```txt
numpy
pandas
scikit-learn
matplotlib
seaborn
flask
streamlit
```

---

# Usage

## Run Prediction Script

```bash
python app.py
```

## Load Saved Model

```python
import pickle

model = pickle.load(open('laptopmodel.pkl', 'rb'))
```

## Example Prediction

```python
sample_input = [[16, 512, 15.6]]
prediction = model.predict(sample_input)
print(prediction)
```

---

# Deployment Options

This project can be deployed using:

* Flask
* Streamlit
* Heroku
* Render
* Railway
* AWS

---

# Future Improvements

* Improve prediction accuracy
* Add deep learning models
* Real-time laptop recommendation system
* Deploy with modern UI
* Add API integration
* Include price trend analysis

---

# Screenshots

Add screenshots of:

* Homepage
* Prediction form
* Output prediction
* Model performance graphs

---

# Learning Outcomes

Through this project, you can learn:

* Data preprocessing
* Regression algorithms
* Feature engineering
* Model serialization
* Machine learning deployment
* End-to-end ML project workflow

---

# Author

**Your Name**

* LinkedIn: [https://linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
* GitHub: [https://github.com/your-username](https://github.com/your-username)

---

# License

This project is licensed under the MIT License.

---

# Conclusion

This Laptop Price Prediction project demonstrates how machine learning can be applied to real-world pricing problems. By analyzing laptop specifications and training regression models, the system can estimate prices with good accuracy and provide practical insights for both buyers and sellers.
