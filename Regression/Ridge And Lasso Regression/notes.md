# Ridge & Lasso Regression  

## 🔹 Concept  
- Ridge & Lasso are **regularized versions of Linear Regression** that prevent overfitting by penalizing large coefficients.  
- **Ridge (L2 penalty):** Shrinks coefficients but keeps all features.  
- **Lasso (L1 penalty):** Shrinks some coefficients to **exactly zero**, performing feature selection.  
- Best used when dataset has multicollinearity (Ridge) or requires feature selection (Lasso).  

---

## 🔹 Key Math  
- **Hypothesis:**  

$$
y = \beta_0 + \beta_1x_1 + \beta_2x_2 + \dots + \beta_nx_n
$$  

- **Ridge Cost Function (L2):**  

$$
J(\theta) = \frac{1}{m} \sum_{i=1}^m (y_i - \hat{y}_i)^2 + \lambda \sum_{j=1}^n \beta_j^2
$$  

- **Lasso Cost Function (L1):**  

$$
J(\theta) = \frac{1}{m} \sum_{i=1}^m (y_i - \hat{y}_i)^2 + \lambda \sum_{j=1}^n |\beta_j|
$$  

---

## 🔹 Steps  
1. **Load dataset** using `pandas.read_csv`.  
2. **Preprocess data**: select features `X` and target `y`.  
3. **Split dataset** into training and testing sets (80:20).  
4. **Train Ridge model** using `Ridge(alpha=λ)`.  
5. **Train Lasso model** using `Lasso(alpha=λ)`.  
6. **Evaluate models** using Mean Squared Error (MSE) and R² Score.  
7. **Tune α (regularization strength)** using `RidgeCV` or `LassoCV`.  
8. **Compare Ridge vs Lasso performance.**  

---

## 🔹 Results (Comparison Table)  

| Metric            | Ridge Regression | Lasso Regression |
|-------------------|------------------|------------------|
| Alpha (λ)         | `XX`             | `XX`             |
| Mean Squared Error| `XX.XXXX`        | `XX.XXXX`        |
| R² Score          | `XX.XXXX`        | `XX.XXXX`        |
| Coefficients      | `[XX, XX, ...]`  | `[XX, XX, ...]`  |
| Intercept         | `XX.XXXX`        | `XX.XXXX`        |

- Screenshot: ![results](output.png)  
