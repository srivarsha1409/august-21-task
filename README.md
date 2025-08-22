**📌 Lasso Regression – Employee Salary Prediction**
**📖 Overview**

This project applies Lasso Regression with Cross-Validation (LassoCV) to predict employee salaries based on multiple factors. The dataset includes various employee attributes such as experience, education, certifications, and soft skills.

The HR team’s challenge:

Not all employee attributes significantly affect salary.

Using all features may lead to overfitting or unnecessary complexity.

Goal: Automatically identify important features while ignoring irrelevant ones.

Lasso Regression is ideal for this scenario because it performs both prediction and feature selection.




**📊 Dataset**

Features (X): experience, education_level, certifications, skills_score, projects_handled, leadership_score, communication_score, location_index, department_index

Target (y): salary_k (salary in thousands)




**
⚙️ Requirements**

Make sure the following Python libraries are installed:

pip install pandas scikit-learn matplotlib




**🚀 Key Steps**

Load and split data

Train/test split to evaluate performance.

Fit LassoCV model

Automatically tunes the regularization parameter (λ).

Performs cross-validation to avoid overfitting.

Feature selection

Coefficients close to 0 → irrelevant features.

Non-zero coefficients → selected by Lasso.

Model evaluation

Compare R² score on training vs. test data.

Visualize feature importance using a bar plot.




**✨ Why Lasso is useful here?**

Automatic feature selection: Lasso shrinks some coefficients exactly to 0, removing unnecessary features.

Simpler model: Easier for HR to understand which factors matter most for salary.

Reduces overfitting: Avoids noise from irrelevant attributes.

Business insight: HR learns whether education, experience, or soft skills play the biggest role in salary decisions.



**🏢 Real-world Impact**

For HR teams:

Build transparent salary prediction systems.

Detect which employee attributes justify salary differences.

Streamline decision-making by ignoring irrelevant data.
