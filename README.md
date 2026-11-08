# Task20
Data Types and Type Conversion Using Python and Pandas

Project Overview

This project focuses on inspecting and converting data types in a Pandas DataFrame using Python.

Correct data types are important for accurate data processing, cleaning, and analysis.

Objective

- Understand different data types in Pandas.
- Inspect column data types using "dtypes".
- Convert columns between strings, integers, floats, booleans, and dates.
- Prepare a clean dataset for further analysis.

Tools and Technologies

- Python
- Pandas
- Jupyter Notebook

Dataset

For this project, a Customer Dataset or Titanic Dataset can be used.

Types of Data Conversion

1. String: Used to store text values.
2. Integer: Used to store whole numbers.
3. Float: Used to store decimal numbers.
4. Boolean: Used to store True or False values.
5. DateTime: Used to store date and time values.

Implementation

Step 1: Import Pandas

import pandas as pd

Step 2: Create a Sample Dataset

data = {
    'Age': ['20', '21', '22'],
    'Salary': ['25000.50', '30000.75', '35000.00'],
    'Customer_ID': ['101', '102', '103'],
    'Subscribed': ['True', 'False', 'True'],
    'Join_Date': ['2026-01-10', '2026-02-15', '2026-03-20']
}

df = pd.DataFrame(data)

Step 3: Inspect Data Types

print(df.dtypes)

Step 4: Convert Data Types

df['Age'] = df['Age'].astype(int)

df['Salary'] = pd.to_numeric(df['Salary'])

df['Customer_ID'] = df['Customer_ID'].astype(int)

df['Subscribed'] = df['Subscribed'].map({
    'True': True,
    'False': False
})

df['Join_Date'] = pd.to_datetime(df['Join_Date'])

Step 5: Check Converted Data Types

print(df.dtypes)
print(df)

Expected Deliverables

- Data-type inspection report.
- Examples of at least four column type conversions.
- Cleaned dataset with appropriate data types.

Conclusion

This project helped me understand how to inspect and convert different data types using Python and Pandas. Proper data types improve data quality and make data processing and analysis easier.

Skills Learned

- Python Programming
- Pandas
- Data Cleaning
- Data Type Conversion
- Data Analysis
