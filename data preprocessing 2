from google.colab import files
uploaded_file = files.upload()

# Import libraries
import pandas as pd
import io

# Read dataset
df = pd.read_csv(io.BytesIO(uploaded_file['water_potability (1).csv']))

print("Shape of dataset :", df.shape)

print("\nTop 5 records")
display(df.head())

print("\nInformation about dataset")
df.info()

print("\nSummary statistics")
display(df.describe())

# Checking missing values
print("\nNull values in each column")
print(df.isna().sum())

# Checking duplicates
dup = df.duplicated().sum()
print("\nNumber of duplicate rows :", dup)
