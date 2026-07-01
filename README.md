# Alfido-task3import pandas as pd

data = {
    "Name": ["Aman", "Riya", "Rahul", "Priya", "Mohit", "Anjali"],
    "Department": ["BCA", "BCA", "BBA", "BCA", "BBA", "BCA"],
    "Marks": [85, 90, 78, 88, 75, 92]
}

df = pd.DataFrame(data)

print("First 5 Rows:")
print(df.head())

print("\nMissing Values:")
print(df.isnull().sum())

print("\nAverage Marks by Department:")
print(df.groupby("Department")["Marks"].mean())

print("\nSummary Statistics:")
print(df.describe())
