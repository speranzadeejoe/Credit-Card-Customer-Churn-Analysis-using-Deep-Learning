# Credit-Card-Customer-Churn-Analysis-using-Deep-Learning

**Credit Card Customer Churn Prediction using Deep Learning**

This project focuses on predicting whether a customer will churn (i.e., stop using the bank's services) using a deep learning model. The objective is to help financial institutions identify at-risk customers and take action to retain them.

---

### 📌 Objective

Build a deep learning model that predicts customer churn based on demographics and banking activity, enabling proactive customer retention strategies.

---

### 📊 Dataset Description

The dataset consists of 10,000 customer records with the following features:

- **RowNumber**: Row index (not used in training)  
- **CustomerId**: Unique ID (not used in training)  
- **Surname**: Customer's surname (not used in training)  
- **CreditScore**: Credit score of the customer  
- **Geography**: Country of residence  
- **Gender**: Male or Female  
- **Age**: Age of the customer  
- **Tenure**: Years as a customer  
- **Balance**: Account balance  
- **NumOfProducts**: Number of bank products used  
- **HasCrCard**: Whether the customer has a credit card (1/0)  
- **IsActiveMember**: Whether the customer is active (1/0)  
- **EstimatedSalary**: Estimated salary  
- **Exited**: **Target variable** – 1 if customer churned, 0 otherwise

---

### 🧠 Model Architecture

The deep learning model is built using Keras (TensorFlow backend) and includes:

- Input layer corresponding to the number of features  
- Hidden layers:  
  - Dense layers with ReLU activation  
  - Dropout layers to reduce overfitting  
- Output layer:  
  - Single neuron with Sigmoid activation for binary classification

---

### 🛠️ Steps Performed

1. **Data Preprocessing**  
   - Dropped irrelevant columns (`RowNumber`, `CustomerId`, `Surname`)  
   - Label encoding for `Gender`, one-hot encoding for `Geography`  
   - Feature scaling (e.g., StandardScaler)  
   - Train-test split (80-20)

2. **Model Training**  
   - Compiled the model with Binary Crossentropy loss and Adam optimizer  
   - Trained using early stopping and validation split  
   - Evaluated on test set

3. **Model Evaluation**  
   - Accuracy  
---

### 📈 Results

_(Update this section after model evaluation)_

Example:
- Accuracy: **85%**  
  

---

### 🔄 Future Improvements

- Hyperparameter tuning with GridSearch or RandomizedSearch  
- Apply class balancing techniques (SMOTE or class weights)  
- Try alternative models like Random Forest, XGBoost for comparison  
- Use SHAP or LIME for model explainability  
- Deploy the model using Streamlit or Flask

---

### 📜 License

This project is licensed under the **MIT License**.

---
