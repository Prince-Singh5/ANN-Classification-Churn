Customer Churn Prediction using ANN 📊🤖

📖 Project Overview
This project is an end-to-end deep learning solution that predicts customer churn — whether a customer will continue using a service or not based on tabular data.
The model is built using an Artificial Neural Network (ANN) architecture, trained on customer attributes and ratings provided in an Excel dataset.

Dataset
Source: Custom Excel dataset.
Features: Customer demographics, ratings, and behavioral attributes.
Target:
  0 → Customer will not continue (churn).
  1 → Customer will continue (retain).

Model Architecture
  model = Sequential()
  model.add(Dense(64, activation='relu', input_dim=feature_count))
  model.add(Dense(32, activation='relu'))
  model.add(Dense(1, activation='sigmoid'))
  
Training
  Optimizer: Adam
  Loss: Binary Crossentropy
  Metrics: Accuracy

🔧 How to Run
  Clone the repository:
    git clone https://github.com/Prince-Singh5/ANN-Classification-Churn.git
  Install dependencies:
    pip install -r requirements.txt
  Run the application
    streamlit run app.py
    
🌟 Key Learnings
  How to preprocess text data with embeddings and RNNs.
  How to preprocess tabular data for ANN training.
  Importance of vocabulary size (num_words=10000) in text models.
  How neural networks can be applied to both NLP and business analytics.

📌 Future Improvements
  Experiment with LSTM/GRU for better text modeling.
  Add dropout/regularization to reduce overfitting.
  Deploy models as web apps or APIs for interactive predictions.
  Compare ANN performance with traditional ML models (Random Forest, XGBoost).
