# Loan Status Prediction - Business Perspective (Story Style)

Imagine you are working at a bank.  
Every day, hundreds of loan applications come in. Some applicants are trustworthy and will pay back, others are risky and may default.  

Traditionally, staff must manually check each application — looking at income, dependents, credit history, etc.  
This process is **slow, inconsistent, and costly**.  

## My Solution
I decided to train a **Machine Learning model** using historical loan data.  
The goal: **predict if a loan should be Approved or Not Approved**.  

I used a **Support Vector Machine (SVM)** model.  
The data was cleaned, missing values removed, and categorical features encoded.  
Finally, the model was trained and tested.

## What I Found
- The model achieves **~83% accuracy** on unseen applicants.  
- For **Approved loans**, recall is **93.9%** → meaning we rarely miss good applicants.  
- For **Not Approved loans**, recall is **60%** → some risky applicants may still slip through.  

This shows the model is **strong at capturing reliable borrowers**, but **needs improvement at detecting risky ones**.

## Business Impact
- **Faster decisions**: Loan approvals can be automated within seconds.  
- **Reduced workload**: Staff can focus on edge cases instead of every file.  
- **Consistent decisions**: Model applies the same logic for all applicants.  

But there’s a challenge:  
- Some risky borrowers might still get approved due to lower recall.  

## Recommendations
- Use **class weighting or alternative algorithms** to improve detection of risky applicants.  
- Combine model predictions with **credit bureau data** for stronger results.  
- Regularly retrain the model with new data to keep it up-to-date.  

## The Big Picture
With this model, the bank gains a **smart assistant**:  
- It never gets tired,  
- It applies rules fairly,  
- It helps the business scale faster.  

This is not just a technical project — it’s a **step towards digital banking transformation**.
