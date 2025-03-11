# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
```
![Screenshot 2025-03-07 111644](https://github.com/user-attachments/assets/9e47be65-1254-48ab-bd1b-dc008ced3c5a)

```
df.head()
```
![Screenshot 2025-03-07 111655](https://github.com/user-attachments/assets/20234c01-4649-48c1-a63b-5cec4ed5d7ba)

```
df.tail()
```
![Screenshot 2025-03-07 111703](https://github.com/user-attachments/assets/57ed5001-e1e4-4ff7-9106-bd975ad5ec9d)

```
df.notnull()
```
![Screenshot 2025-03-07 111815](https://github.com/user-attachments/assets/e3966742-b8e3-4d55-ba12-65bc7febeaa4)

```
df.isnull()
```
![Screenshot 2025-03-07 111830](https://github.com/user-attachments/assets/04e872bc-8c16-43d8-8358-e0452c12c899)
```
df.fillna(5)
```
![Screenshot 2025-03-07 111848](https://github.com/user-attachments/assets/49c51779-82ad-4eae-9b38-db6ff913daa6)
```
df.dropna(axis=0)
```
![Screenshot 2025-03-07 111925](https://github.com/user-attachments/assets/124cb19b-501a-4a4a-a6b6-112e1a6e6726)

```
df.dropna(axis=1)
```
![Screenshot 2025-03-07 111930](https://github.com/user-attachments/assets/a8b46775-3730-4a33-8439-3d9c5d81f072)
```
df.isnull().sum()
```
![Screenshot 2025-03-07 111935](https://github.com/user-attachments/assets/393eba36-9c1c-4073-bb44-f09796ea5d0f)
```
df.isnull().any()
```
![Screenshot 2025-03-07 111941](https://github.com/user-attachments/assets/5e841b29-e166-4eba-b5f0-280d696498cb)
```
df.fillna(method='ffill')
```
![Screenshot 2025-03-07 111949](https://github.com/user-attachments/assets/23180a7d-2665-4212-86d3-58a8cf01af3d)
```
df.fillna(method='bfill')
```
![Screenshot 2025-03-07 111954](https://github.com/user-attachments/assets/85b50ff3-3e6f-4b9f-a6c9-cb5834c2428f)

```
df.fillna({'NAME':'THRISHANTH','M4':55,'TOTAL':420.0})
```
![Screenshot 2025-03-07 112002](https://github.com/user-attachments/assets/a341e5d2-7cb8-4372-88a1-d03bd2d8b956)
![Screenshot 2025-03-07 112007](https://github.com/user-attachments/assets/5e9642f4-66c3-44c7-b3d8-b509b8006dcf)
![Screenshot 2025-03-07 112011](https://github.com/user-attachments/assets/06965428-17f1-455c-a3f7-7c63a27fa627)
![Screenshot 2025-03-07 112017](https://github.com/user-attachments/assets/baef2cf5-f2fd-438d-9c9b-eafb110a443b)
![Screenshot 2025-03-07 112035](https://github.com/user-attachments/assets/25ede72c-655e-47a6-8e29-35d105b62125)
![Screenshot 2025-03-07 112041](https://github.com/user-attachments/assets/37152137-6ddb-408b-98ba-a63deb35dd5c)
![Screenshot 2025-03-07 112045](https://github.com/user-attachments/assets/40ac850d-c56d-4ffa-9632-c16587a7c893)
![Screenshot 2025-03-07 112053](https://github.com/user-attachments/assets/d2b5f23e-a85b-4f29-b805-77464b318a71)
![Screenshot 2025-03-07 112102](https://github.com/user-attachments/assets/6bb4ace9-989b-453a-9779-bc8df46e2460)
![Screenshot 2025-03-07 112107](https://github.com/user-attachments/assets/cbc87889-1ca9-4939-ae76-e2c28e85e955)
![Screenshot 2025-03-07 112113](https://github.com/user-attachments/assets/7b48113f-b6c9-4692-a2cd-e58ccf0cbb26)
![Screenshot 2025-03-07 112119](https://github.com/user-attachments/assets/3c815d75-f52b-4af5-9fe8-ebf8a215f3c9)
![Screenshot 2025-03-07 112130](https://github.com/user-attachments/assets/4890bee3-836a-4cb5-a848-aa018ead2fe5)
![Screenshot 2025-03-07 112134](https://github.com/user-attachments/assets/5254a65c-f62c-458f-93f0-57c61a8deead)
![Screenshot 2025-03-07 112138](https://github.com/user-attachments/assets/860c6da8-1c1d-4b6c-99b9-0463020112cf)







# Result
       Thus the given data is read and data cleaning is performed.
