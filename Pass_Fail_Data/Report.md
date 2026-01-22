# Report File Based on data analysis
Student Pass-Fail Data Analysis 

## 1. Project Overview
This project analysis a student performance dataset (Pass-Fail Data) to understand the key factors that influence whether the student passes or fails an exam.

The dataset contains the following features :
- student_id
- attendance
- homework_pct
- midterm_score
- study_hours_per_week
- pass(0 = Fail, 1 = Pass)

All numerical features are in integer format, and the target variable `pass` is binary.
The analysis was performed using **Python, Pandas, Numpy, Matplotlib, Seaborn**.

---

## 2. Objectives
The main objective of this analysis are:
- To explore and clean the dataset.
- To compare academic and behaviour factor between passed and failed students.
- To identify which feature have the Strongest impact on the student success.
-To visualize the patterns and relationship in the data.

---

## 3. Data Exploration & Cleaning
- Loaded the dataset using pandas and inspected its structure using several functions.
- Checked the missing values and duplicate records.

- No major inconsistencies were found in the dataset.

---

## 4. Exploring Data Analysis (EDA)
### 4.1 Pass vs Fail Distribution
- Counted the number of passed and failed students using `value_counts()`.  
- Visualized the distribution using a bar chart.

**Observation:**  
The dataset shows a balanced / moderately imbalanced distribution between pass and fail categories.

### 4.2 Comparison of Academic Factors
Grouped the data by `pass` and calculated mean values:

- Passed students had:
  - Higher average attendance  
  - Higher homework completion percentage  
  - Higher midterm scores  
  - Higher weekly study hours  

This indicates that consistent academic effort is strongly associated with passing.

### 4.3 Study Hours and Attendance Analysis
Boxplots were created to compare:

- Study hours vs Pass/Fail  
- Attendance vs Pass/Fail  

*Observations:*

- Students who passed generally studied more hours per week.  
- Attendance showed a clear separation between passed and failed students.  
- Attendance appears to be one of the strongest indicators of success.

---

## 5. Correlation Analysis
A correlation matrix and heatmap were generated to measure realationships between variables.

**Key Finding**

- `midterm_score` has the strongest positive correlation with `pass`.  
- `attendance` also shows a strong positive correlation with passing.  
- `study_hours_per_week` has a moderate positive correlation.  
- `homework_pct` has a positive but comparatively weaker correlation.

*Conclusion:*  
Midterm performance and attendance are the most influential factors for passing the exam.

--- 

## 6. Feature Enginnering
Additional features were created for deeper analysis:
- **Performance score**
- **Hardworking Flag**

*Observation:*
- Most Student labled as "hardworking" had a higher probability of passing.
- The performance score clearly separated pass and fail groups.

---

## 7. Key Insights

- Students with higher attendance and midterm scores are significantly more likely to pass.  
- Attendance plays a more critical role than homework percentage.  
- Study hours positively impact performance, but alone are not sufficient without good attendance and exam scores.  
- A combination of consistent attendance, regular study, and strong exam performance leads to the highest success rate.

---

## 8. Tools & Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 9. Conclusion

This project demonstrates how exploratory data analysis and visualization can be used to identify important academic factors affecting student success.

The analysis shows that **attendance and exam performance are the strongest predictors of passing**, while study habits further improve outcomes.

This project can be extended in the future by:

- Applying machine learning classification models (Logistic Regression, Decision Tree)  
- Predicting pass/fail outcomes for new students  
- Performing feature importance analysis  

---

## 10. Author

**Hari Sharma**  
Aspiring Data Analyst & Developer  
GitHub: https://github.com/harix28  
LinkedIn: https://www.linkedin.com/in/hari-sharma-73637a2b1  
