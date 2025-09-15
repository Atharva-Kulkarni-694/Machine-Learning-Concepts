# Logistic Regression

## 🔹 Concept
- Logistic Regression is a **supervised classification algorithm** used to predict a binary outcome (0/1, True/False).  
- It models the probability of belonging to a particular class using the **sigmoid function**.  
- Best used when the dependent variable is categorical (e.g., defect/no defect, spam/not spam).  

## 🔹 Key Math
- **Hypothesis function:**  

$$
P(y=1|x) = \frac{1}{1 + e^{-(\beta_0 + \beta_1x_1 + \beta_2x_2 + \dots + \beta_nx_n)}}
$$  

- **Cost function (Log Loss):**  

$$
J(\theta) = -\frac{1}{m} \sum_{i=1}^m \left[ y_i \log(\hat{y}_i) + (1-y_i)\log(1-\hat{y}_i) \right]
$$  

- **Optimization method:** Gradient Descent / Maximum Likelihood Estimation (solved internally by `sklearn`).  

## 🔹 Steps
1. **Load dataset** using `pandas.read_csv`.  
2. **Preprocess data**: select feature columns `X` and binary target `y`.  
3. **Split dataset** into training and testing sets (80:20).  
4. **Train model** using `LogisticRegression()` from `sklearn`.  
5. **Evaluate model** using accuracy, confusion matrix, and classification report.  
6. **Plot results**:  
   - For single feature → plot logistic curve.  
   - For multiple features → plot ROC curve with AUC.  

## 🔹 Results
- Accuracy: `XX.XXXX`  
- Precision: `XX.XXXX`  
- Recall: `XX.XXXX`  
- F1-Score: `XX.XXXX`  

- Confusion Matrix:  



- Classification Report:  




- Screenshot: ![results](output.png)  
