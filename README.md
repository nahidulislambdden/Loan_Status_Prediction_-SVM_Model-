# Loan Status Prediction

This project predicts whether a loan application will be **Approved or Not Approved** based on applicant details using a **Support Vector Machine (SVM)** classifier.

## 🔹 Project Workflow
1. **Data Collection & Preprocessing**
   - Missing values handled (dropped in this version).
   - Encoding of categorical features (e.g., Gender, Married, Education).
   - Target variable (`Loan_Status`) encoded (Y=1, N=0).

2. **Exploratory Data Analysis (EDA)**
   - Countplots used to visualize education, marital status vs. loan approval.

3. **Feature Engineering**
   - Final features: Gender, Married, Dependents, Education, Self_Employed,  
     ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term,  
     Credit_History, Property_Area.

4. **Train-Test Split**
   - 90% train (432 samples), 10% test (48 samples).

5. **Model Training**
   - Classifier: Support Vector Machine (SVM, linear kernel).

6. **Evaluation**
   - Accuracy (train): ~79.9%  
   - Accuracy (test): ~83.3%  
   - Classification Report & Confusion Matrix generated.

7. **Business Demo**
   - Prediction for a new applicant profile.

## 🔹 Results
- **Training Accuracy**: ~79.9%  
- **Test Accuracy**: ~83.3%  
- **Approved (class=1)**: Precision 0.838, Recall 0.939 → strong.  
- **Not Approved (class=0)**: Precision 0.818, Recall 0.600 → weaker.  
- **Overall Conclusion**: Model is reliable for identifying approved loans but needs tuning to catch more risky borrowers.

## 🔹 Business Impact
- Automates loan approval process → faster decisions.  
- Reduces manual workload for banking staff.  
- Minimizes missed opportunities (good applicants rarely rejected).  
- Still needs improvement to reduce risky approvals.  

## 🔹 How to Run
```bash
# clone the repository
git clone https://github.com/<your-username>/Loan_Status_Prediction.git
cd Loan_Status_Prediction

# install dependencies
pip install -r requirements.txt

# open the notebook
jupyter notebook Loan_Status_Prediction.ipynb
