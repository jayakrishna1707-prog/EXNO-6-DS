# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding

```
import seaborn as sns
import matplotlib.pyplot as plt
df=sns.load_dataset("iris")
df.head()
corr_matrix=df.select_dtypes(include=["float64"]).corr()
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm")
plt.show()
sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='hex')
sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='reg')
sns.pairplot(df)
sns.pairplot(df,hue='species')
sns.distplot(df['sepal_width'])
sns.distplot(df['petal_length'],kde=False,bins=10)
sns.countplot(x='species',data=df)
sns.countplot(y='species',data=df)
sns.barplot(x='sepal_length',y='sepal_width',data=df)
sns.boxplot(x='sepal_length',y='sepal_width',data=df)
sns.boxplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')
sns.boxplot(data=df,orient='v')sns.boxplot(x='sepal_length',y='sepal_width',data=df,hue='species')
sns.violinplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')

```

# Output

![alt text](<Screenshot 2026-03-16 202906.png>)
![alt text](<Screenshot 2026-03-16 202916.png>)
![alt text](<Screenshot 2026-03-16 202935.png>)
![alt text](<Screenshot 2026-03-16 202948.png>)
![alt text](<Screenshot 2026-03-16 203012.png>)
![alt text](<Screenshot 2026-03-16 203027.png>)
![alt text](<Screenshot 2026-03-16 203038.png>)
![alt text](<Screenshot 2026-03-16 203048.png>)
![alt text](<Screenshot 2026-03-16 203058.png>)
![alt text](<Screenshot 2026-03-16 203107.png>)
![alt text](<Screenshot 2026-03-16 203117.png>)
![alt text](<Screenshot 2026-03-16 203125.png>)
![alt text](<Screenshot 2026-03-16 203134.png>)
![alt text](<Screenshot 2026-03-16 203143.png>)
![alt text](<Screenshot 2026-03-16 203152.png>)
![alt text](<Screenshot 2026-03-16 203201.png>)


# Result:
 
 Thus,The data visualization using seaborn library is completed successfully
