# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE 
# For Data_set
```
 import pandas as pd
 df=pd.read_csv("/content/Data_set .csv")
 df

 df.head(10)

 df.info()

 df.isnull()

 df.isnull().sum()

 df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
 df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
 df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
 df.head()

 df['rating']=df['rating'].fillna(df['rating'].mean())
 df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean
 df.head()

 df['watchers']=df['watchers'].fillna(df['watchers'].median())
 df.head()

 df.info()

 df.isnull().sum()
```
# For loan_set
```
 import pandas as pd
 df=pd.read_csv("/content/Loan_Data.csv")
 print(df)

 df.head(5)

 df.info()

 df.isnull()

 df.isnull().sum()

 df['Loan_ID']=df['Loan_ID'].fillna(df['Education'].mode()[0])
 df['Education']=df['Education'].fillna(df['Education'].mode()[0])
 df['Married']=df['Married'].fillna(df['Education'].mode()[0])
 df.head()

 df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
 df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())
 df.head()

 df.head()

 df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].median())
 df.head()

 df.info()

 df.isnull().sum()
```
# OUTPUT
# For Data_Set
# DATA
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/5ba9ad25-6468-4676-8c9c-865392228022)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/566ab26e-4369-44e1-83b7-c58cb672e98b)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/6407cd96-9d68-4d5f-a26e-8f05ad1ce11a)
# NON NULL BEFORE
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/ab64a2d5-882b-42a7-8880-8d326e979d7d)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/3c3d04ac-99dc-49d8-8717-95a3a754d96d)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/5b3d1e59-f1c0-42f6-80b8-89bf25a6c98c)
# MODE
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/2242e8c8-94e3-420d-a5c5-d5a941567464)
# MEAN
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/e104525d-d256-486a-96a4-8ecb4af595a7)
# MEDIAN
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/b7fdfb0d-93b7-4eb2-a101-78d13a568875)
# NON NULL AFTER
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/33f14226-a58d-496f-83de-e51abcf2b884)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/76b50a5b-6e44-4fed-bbe6-80f5a9272321)
# For loan_data
# DATA
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/4c39d3e9-82ca-44b0-956a-fe06ab63499d)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/82c5ce48-4ac5-427c-bb95-08322034c5c6)
# NON NULL BEFORE
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/9d58efe0-72a7-4051-900e-06cf0a59990c)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/cea80978-87d6-41fd-8d3d-c3107bbff9d7)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/f6bfea13-debd-4195-9f7e-52d9bbab9eed)
# MODE
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/ec74e579-181f-42ce-907e-eb025d2a1f86)
# MEAN
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/48a22a5b-ec02-4407-b649-f71e6070bd9d)
# MEDIAN
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/ca0ab3e6-9dc9-4e57-80c9-9f62ac78cb6b)
# NON NULL AFTER
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/a27ace9a-a294-4070-bca6-29f349a9af6c)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex01/assets/131433133/154af51d-7d7c-4cd9-90fe-f4e60656b740)
#  RESULT
Thus, the given data is read, cleansed and the cleaned data is saved into the file.

























 
