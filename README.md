# Mini-Project

## Credit Data Analysis

## Aim 
To perform analysis Of Credit Data using basic data science techniques.

## Algorithm
Step 1 Import necessary packages
Step 2 Read the data set
Step 3 Execute the methods
Step 4 Run the program
Step 5 Get the output

## Code
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("/content/credit_data_1.csv")
df
df.head()
df.info()
df.tail()
df.describe()
df.shape
df['dependents'].value_counts()
from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()

df['dependents'] = le.fit_transform(df['dependents'])
df.head(10)
df.isnull().sum()
missing_percentage = (df.isnull().sum())/(df.shape[0])*100
missing_percentage
df.duplicated().value_counts()
sns.boxplot(y="dependents",data=df)
sns.countplot(y="dependents",data=df)
sns.histplot(y="dependents",data=df)
sns.scatterplot(df['income'],df['expenditure'])
sns.barplot(data=df, x='income', y='owner')
df.corr()
sns.heatmap(df.corr(),annot=True)
plt.figure(figsize=(20, 7))
sns.lineplot(data=df, x='age', y='expenditure')
plt.show()
sns.kdeplot(x=df['active'],data=df)
sns.countplot(y="card",data=df)
```

## Output

## Importing dataset
<img width="610" alt="s1" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/0800412c-a92d-4b91-85e7-ebaaadac9298">

## head
<img width="611" alt="s2" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/dd1f8c64-bca6-4263-a3c5-7c83b9125082">

## info
<img width="316" alt="s3" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/d3f38c71-1494-4012-a8f2-2fe98fb785e6">

## tail
<img width="599" alt="s4" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/dbd8641b-e680-4444-ba97-77f07376dcd8">

## describe
<img width="598" alt="s5" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/a8b283ab-bddd-4b08-a34b-742755a9af4b">

## shape
<img width="109" alt="s6" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/ce9c7b41-cf27-40e8-9128-193a9d9b3642">

## dependents
<img width="242" alt="s7" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/afdad84d-4116-4c24-ac91-c7cec800e3c7">

## Label Encoder:
<img width="605" alt="s8" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/8018213b-9542-4932-8372-d81ea6c49cea">

## Data Exploratory Analysis:

## null values
<img width="146" alt="s9" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/45b09054-ac61-43dd-aeb8-281a7e761370">

## missing_percentage
<img width="194" alt="s10" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/19403a31-1ef8-488f-afcc-8c4608b25349">

## duplicates
<img width="126" alt="s11" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/997dc3c0-f014-4e13-8746-f0baf56a9f51">

## Univariate Analysis:

## boxplot
<img width="419" alt="s12" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/abdea83c-6fa2-4dfb-82b5-16af0d5f72eb">

## countplot
<img width="418" alt="s13" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/6b4274c8-f1e7-4b87-9d76-bdeb6ea4e5fe">

## histplot
<img width="420" alt="s14" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/53aa7981-d6f1-4599-84fc-d88445ed1075">

## Multivariate Analysis:

## scatterplot
<img width="435" alt="s15" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/222b1c70-7c3f-4ec1-a042-dfa6e868347f">

## barplot
<img width="431" alt="s16" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/81ae89b8-e3b1-4b99-b163-3c556dece38e">

## heatmap
<img width="486" alt="s17" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/09137786-5ba6-45d3-b5a3-14d8d5b4826b">

<img width="398" alt="s18" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/a90277e2-4e94-4726-ab75-cbf0e768b6e6">

## Data Visualization:

## lineplot
<img width="418" alt="s19" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/cb6814d9-ed1b-431b-acc7-26356c6f8b22">

## kdeplot
<img width="356" alt="s20" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/ee830cf7-0887-47c8-88c2-a72abd5a47db">

## countplot
<img width="346" alt="s21" src="https://github.com/SmritiManikand/Mini-Project/assets/113674204/084dbae5-16ba-4555-b549-51f16ed63cdb">

## Result
Hence the program to analyze the data set using data science is implemented successfully.
