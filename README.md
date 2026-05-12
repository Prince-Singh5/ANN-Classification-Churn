# Customer Churn Prediction using ANN 📊🤖

## 📖 Project Overview
This project is an end-to-end deep learning solution that predicts **customer churn** — whether a customer will continue using a service or not — based on tabular data.  
The model is built using an **Artificial Neural Network (ANN)** architecture, trained on customer attributes and ratings provided in an Excel dataset.

---

## ⚙️ Dataset
- **Source**: Custom Excel dataset  
- **Features**: Customer demographics, ratings, and behavioral attributes  
- **Target**:  
  - `0` → Customer will not continue (churn)  
  - `1` → Customer will continue (retain)  

### Preprocessing
- Data cleaning and normalization  
- Conversion into numerical format suitable for ANN training  
- Train-test split applied for evaluation  

---

## 🏗️ Model Architecture
```python
model = Sequential()
model.add(Dense(64, activation='relu', input_dim=feature_count))
model.add(Dense(32, activation='relu'))
model.add(Dense(1, activation='sigmoid'))
