# Bank-Loan-Prediction
Machine learning model to predict bank loan approvals.

# Bank Loan Prediction 🏦

This project uses Machine Learning to predict whether a bank loan should be approved or rejected based on the applicant's profile. The model considers various factors like income, loan amount, credit history, and employment status.

## 📊 Dataset
The dataset used in this project is `Bank_Loan.csv`. It contains the following details:
* **Applicant Information:** Gender, Marital Status, Education, Dependents, and Self-Employment status.
* **Financial Metrics:** Applicant Income, Co-applicant Income, and Loan Amount.
* **Loan Details:** Loan Amount Term, Credit History, and Property Area.
* **Target Variable:** `Loan_Status` (Y/N - indicating whether the loan was approved).

## 🚀 Features & Workflow
The Jupyter Notebook (`LoanPrediction.ipynb`) follows a structured Data Science workflow:

1. **Data Exploration:** Exploring random rows, top/bottom rows, and checking overall dataset statistics.
2. **Data Preprocessing:**
   * Finding and removing duplicate records.
   * Dropping unwanted columns (like `Loan_ID`).
   * Categorical to numerical data conversion.
3. **Feature Scaling:** Normalizing features like `ApplicantIncome`, `CoapplicantIncome`, and `LoanAmount` using `MinMaxScaler`. The scaler is saved as `scaler.pkl` for future predictions.
4. **Handling Class Imbalance:** Addressing the loan status class imbalance to prevent model bias.
5. **Model Training & Testing:** The dataset is split into training and testing sets, and the following Machine Learning models are trained:
   * **Random Forest Classifier**
   * **Support Vector Machine (SVM)**
   * **K-Nearest Neighbors (KNN)**
6. **Model Validation:** * Accuracy Score evaluation.
   * Confusion Matrix visualization using `seaborn` and `matplotlib`.
   * Classification Report (Precision, Recall, F1-Score).

## 🛠️ Technologies Used
* **Python** 3.x
* **Pandas & NumPy:** Data manipulation and analysis.
* **Matplotlib & Seaborn:** Data visualization.
* **Scikit-Learn:** Machine learning algorithms, data splitting, and evaluation metrics.

## 📈 Results
The models were evaluated using accuracy scores on the test dataset. The performance of the models is as follows:

* **Random Forest Classifier:** ~91.43% Accuracy 
* **K-Nearest Neighbors (KNN):** ~88.57% Accuracy
* **Support Vector Machine (SVM):** 80.00% Accuracy

The **Random Forest Classifier** was the best-performing model, achieving high precision and recall for both loan approval and rejection categories.

## 📂 Files Included
* `Bank_Loan.csv`: The dataset file.
* `LoanPrediction.ipynb`: Jupyter notebook containing the complete python code and outputs.

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/kishorekumarS26/Bank-Loan-Prediction.git]
