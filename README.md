# Customer Churn Prediction 📉🤖

This project leverages an **Artificial Neural Network (ANN)** to predict customer churn based on historical data. Customer churn is a critical metric in industries like telecommunications, banking, and SaaS, and this project demonstrates how machine learning can effectively address this problem.

---

## 🚀 Features

- Predicts whether a customer will churn or remain loyal based on input data.
- Utilizes a custom **ANN** implemented in Python with **TensorFlow/Keras**.
- Preprocessing of categorical and numerical data for optimal model performance.
- Provides insights into customer behavior via exploratory data analysis (EDA).
- Easy-to-follow **Jupyter Notebook** implementation for training, evaluation, and prediction.

---

## 📂 Project Structure

```plaintext
customer-churn-prediction/
│
├── data/                  # Dataset folder
│   └── churn_data.csv     # Customer churn dataset
├── notebooks/             # Jupyter Notebooks
│   └── churn_prediction.ipynb  # Main implementation
├── models/                # Saved ANN models
├── README.md              # Project documentation (this file)
├── requirements.txt       # Python dependencies
└── utils/                 # Utility scripts for preprocessing and visualization
```
## 🏗️ Model Architecture

The Artificial Neural Network (ANN) for customer churn prediction is designed as follows:

1. **Input Layer**:
   - Processes preprocessed customer data, including demographic, service usage, and account information.

2. **Hidden Layers**:
   - **Layer 1**: Fully connected dense layer with 128 neurons, using ReLU activation.
   - **Layer 2**: Dropout layer (rate = 0.3) to reduce overfitting.
   - **Layer 3**: Dense layer with 64 neurons and ReLU activation.

3. **Output Layer**:
   - Fully connected dense layer with a single neuron.
   - Uses a sigmoid activation function for binary classification (0 = No Churn, 1 = Churn).

4. **Loss Function**:
   - Binary Cross-Entropy for minimizing error in classification.

5. **Optimizer**:
   - Adam Optimizer for adaptive learning rates.

6. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, and F1-Score.
