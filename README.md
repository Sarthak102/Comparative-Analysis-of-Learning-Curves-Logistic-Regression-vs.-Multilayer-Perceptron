# **Customer Churn Prediction: A Comparative Analysis of Logistic Regression and Multilayer Perceptron**

This project compares the learning curves of two machine learning algorithms, Logistic Regression and Multilayer Perceptron (MLP), for predicting customer churn in an e-commerce context. The analysis evaluates the convergence behavior and generalization performance of both models, providing insights into their strengths and limitations when applied to real-world data.

## **Table of Contents**
- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## **Introduction**

Customer churn prediction is a crucial aspect of customer retention strategies in competitive markets like e-commerce. By predicting which customers are likely to leave, companies can proactively engage with those at risk and implement retention measures. This project uses Logistic Regression and Multilayer Perceptron to predict churn and compare their performance based on learning curves, accuracy, and other evaluation metrics.

The project demonstrates:
- The simplicity and speed of Logistic Regression, which provides a quick baseline with high interpretability.
- The advanced capabilities of MLP, which captures complex, non-linear relationships in the data but requires more computational resources.

## **Features**
- Preprocessing of customer data: missing value handling, encoding, and scaling.
- Implementation of two machine learning models: Logistic Regression and MLP.
- Performance evaluation using accuracy, precision, recall, and F1-score.
- Visualization of learning curves to compare the models' convergence behavior.

## **Dataset**
The dataset used for this project is `data_ecommerce_customer_churn.csv`, which includes customer attributes such as:
- **Tenure**: The number of months a customer has been with the company.
- **WarehouseToHome**: Distance from the warehouse to the customer’s home.
- **SatisfactionScore**: A rating of the customer’s satisfaction level.
- **Churn**: The target variable indicating if a customer has churned (1) or not (0).

## **Installation**

To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

## **Usage**

1. **Load the dataset**:
   The project expects the dataset to be located at the specified path. Modify the path in the code if needed:
   ```python
   data = pd.read_csv('data_ecommerce_customer_churn.csv')
   ```

2. **Run the Jupyter Notebook or Python script**:
   - If using a Jupyter Notebook, execute the cells sequentially to perform data preprocessing, model training, evaluation, and visualization.
   - If using a Python script, run it using:
     ```bash
     python script_name.py
     ```

3. **Evaluate Model Performance**:
   The code will output accuracy, precision, recall, and F1-score for both models, along with learning curves that visually compare their convergence and generalization.

## **Model Details**

### **Logistic Regression**
- **Description**: A linear model for binary classification that predicts the probability of a binary outcome.
- **Accuracy**: 88.84%
- **Strengths**: Fast, interpretable, and effective for linearly separable data.

### **Multilayer Perceptron (MLP)**
- **Description**: A neural network model with hidden layers capable of learning non-linear patterns in the data.
- **Accuracy**: 93.79%
- **Strengths**: High predictive power and ability to capture complex relationships.

## **Results**
- **Learning Curves**: MLP shows slower convergence but achieves higher accuracy and recall than Logistic Regression, making it more suitable for capturing complex patterns in customer data.
- **Generalization Performance**: MLP demonstrates superior generalization with higher recall, reducing false negatives in churn prediction.

## **Contributing**
Contributions are welcome! Please follow these steps if you wish to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.
