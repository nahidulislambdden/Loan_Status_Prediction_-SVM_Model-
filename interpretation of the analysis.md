# Loan Status Prediction - Code Interpretation

## 1. Importing Dependencies
- **numpy, pandas** → numerical operations & data handling  
- **matplotlib, seaborn** → visualization  
- **train_test_split** → splitting dataset into training/testing  
- **svm** → Support Vector Machine classifier  
- **accuracy_score, confusion_matrix, classification_report** → evaluation metrics  

## 2. Data Collection & Processing
- Dataset loaded (614 rows, 13 columns).  
- Missing values dropped → dataset reduced to 480 rows.  
- Target variable `Loan_Status` encoded (`Y=1, N=0`).  
- Categorical columns (Gender, Married, Education, Self_Employed, Property_Area) converted to numeric.  

## 3. Data Visualization
- Countplots used to check relationship of education/marital status with loan approval.  
- Insight: graduates & married applicants had higher approval.  

## 4. Train-Test Split
- Features (X): 11 applicant details.  
- Target (Y): Loan_Status (0 = Not Approved, 1 = Approved).  
- Split: 90% training (432), 10% testing (48).  
- Stratified sampling ensured class balance.  

## 5. Model Training
- Model: **SVM with linear kernel**.  
- Trained using 432 samples.  

## 6. Model Evaluation
- Training Accuracy: ~79.9%  
- Test Accuracy: ~83.3%  
- Model shows good generalization.  

## 7. Predictions
- Test set predictions generated.  
- Example: first applicant predicted as **Approved**.  
- New applicant profile also predicted successfully.  

## 8. Confusion Matrix + Report
- True Positives = 31  
- True Negatives = 9  
- False Positives = 6  
- False Negatives = 2  

**Classification Report**:  
- Approved (1): Precision 0.838, Recall 0.939 → strong detection.  
- Not Approved (0): Precision 0.818, Recall 0.600 → weaker detection.  
- Overall Accuracy: ~83%.  
