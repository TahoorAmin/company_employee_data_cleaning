Company Employee Data Cleaning

📌 Project Overview: 
This project focuses on cleaning and preparing a messy company employee dataset using Python and Pandas. The dataset was inspected to identify common data quality issues, and appropriate data cleaning techniques were applied to make the dataset consistent, complete, and suitable for further analysis.
The project also includes a comparison of the dataset before and after cleaning and exports the final cleaned dataset as a CSV file.

🎯 Objective: 

The main objective of this project is to:
- Load and inspect a messy company employee dataset.
- Identify missing values.
- Identify and correct inconsistent entries.
- Identify and correct inappropriate data types.
- Identify and remove duplicate records.
- Apply suitable data cleaning techniques based on the nature of each problem.
- Verify the dataset after cleaning.
- Compare the dataset before and after cleaning.
- Export the final cleaned dataset as a CSV file.
- Document the cleaning steps performed.

🛠️ Technologies Used:
- Python
- Pandas
- Jupyter Notebook / VS Code
- CSV
- 
📂 Dataset:

The dataset contains company employee information, including fields such as:
- Employee ID
- Employee Name
- Department
- Job Title
- Age
- Gender
- Annual Salary
- Experience Years
- Joining Date
- City
- Performance Score
- Work Mode

The original dataset contains several data quality issues that need to be addressed before further analysis.

🔍 Data Cleaning Process:

1. Dataset Loading and Inspection:
The dataset was loaded using Pandas and initially inspected using functions such as:
- "head()"
- "info()"
- "describe()"
- "isna().sum()"
- "unique()"
- "duplicated()"

This helped in understanding the structure of the dataset and identifying potential data quality problems.

2. Handling Incorrect Data Types:

The "Joining Date" column was initially stored as a string/object data type.
It was converted into the appropriate datetime format using Pandas so that the column could be correctly interpreted and used for date-related analysis.
Other columns were already stored in suitable data types and did not require unnecessary conversion.

3. Handling Missing Values:

Missing values were identified using:
df.isna().sum()
The missing values were handled using appropriate techniques depending on the nature of each column.

Methods used included:
- Mean imputation
- Mode imputation
- Other suitable missing-value handling techniques where required

The cleaned dataset was then checked again to verify that the missing values had been handled successfully.

4. Handling Inconsistent Entries:

Categorical columns were inspected for inconsistent representations of the same values.
For example, variations in capitalization or formatting were standardized so that the same category was represented consistently throughout the dataset.
This improved the consistency and reliability of the categorical data.

5. Handling Duplicate Records:

Duplicate records were identified using:
df.duplicated().sum()
The duplicate records were removed using:
df_cleaned = df_cleaned.drop_duplicates()
The dataset was then checked again to confirm that duplicate records had been removed.

✅ Verification:
After the cleaning process, the dataset was rechecked to verify the improvements.


📊 Before and After Comparison:
The original dataset and cleaned dataset were compared to evaluate the effect of the cleaning process.

💡 Conclusion
The project demonstrates the importance of data cleaning as an essential step before performing data analysis or building machine learning models. By identifying missing values, inconsistent entries, inappropriate data types, and duplicate records, the dataset was transformed into a cleaner and more reliable form.

The final cleaned dataset was exported successfully for further use.

# Author:
Tahoor Amin 
BSc Data Science Student
