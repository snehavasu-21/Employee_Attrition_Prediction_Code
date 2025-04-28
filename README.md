📄 Employee Attrition Analysis and Prediction
🧩 Project Title:
Employee Attrition Analysis and Prediction

🧠 Objective:
The goal of this project is to perform a detailed analysis of employee data to understand the factors influencing employee attrition and to build a predictive model that can predict whether an employee is likely to leave the organization.

📚 Dataset Description:
The dataset includes various features about employees, such as:

Demographics: Age, Gender, Marital Status

Job Information: Department, Job Role, Job Level, Work Experience

Performance Metrics: Performance Rating, Job Satisfaction, WorkLife Balance

Compensation Details: Monthly Income, Stock Option Level, Salary Hike

Other: Overtime Status, Distance from Home, Training Times

The target column for prediction is Attrition — whether an employee leaves (Yes) or stays (No).

🛠️ Tools and Technologies Used:
Python 3

Google Colab

Libraries:

pandas for data handling

numpy for numerical computations

seaborn and matplotlib for visualization

scikit-learn for machine learning

🔎 Exploratory Data Analysis (EDA):
Data Cleaning: Identified non-numeric columns that could not be used directly for correlation.

Correlation Analysis:

Numeric features were extracted and a heatmap was plotted.

This showed the relationships between numerical factors.

Observations:

Higher TotalWorkingYears seemed associated with longer YearsAtCompany.

MonthlyIncome had some positive correlation with JobLevel and TotalWorkingYears.

🏗️ Data Preprocessing:
Non-numeric columns (like BusinessTravel, Department, etc.) would be encoded if full modeling was needed.

Only numeric columns were used initially for analysis to avoid conversion errors.

Missing values were not present (since the provided data was clean).

🔮 Model Building:
(Optional: full model would need multiple data samples for training.)

In this specific task:

Since only one new input row was provided, full model training was not performed.

Normally, we would:

Split the dataset into train-test sets

Encode categorical variables

Train classifiers like Logistic Regression, Random Forest, or XGBoost

Evaluate with accuracy, precision, recall, and F1-score

🧪 Testing with New Input:
A sample employee record was tested:


Feature	Value
Age	56
BusinessTravel	Travel_Rarely
Department	Research & Development
EducationField	Life Sciences
Gender	Male
JobRole	Manufacturing Director
MaritalStatus	Single
MonthlyIncome	7260
OverTime	No
TotalWorkingYears	37
YearsAtCompany	6
Prediction Target: Attrition → No

📈 Visualizations:
Heatmap of numeric feature correlation was plotted using Seaborn.

Highlighted stronger and weaker feature associations visually.

✅ Conclusion:
The employee dataset includes rich information across demographics, job metrics, and salary features.

Numeric features must be separated for direct correlation analysis.

Text columns (categorical data) must be encoded for full machine learning models.

The project successfully handled real-world issues such as mixed data types during EDA.

A predictive model can be built with full datasets following proper preprocessing steps.

📂 Future Work:
Implement full Label Encoding or One-Hot Encoding for categorical variables.

Train and tune a classification model (Random Forest, XGBoost, Logistic Regression).

Evaluate using cross-validation.

Deploy the model as an API for real-time employee attrition prediction.
