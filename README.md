# Ex-09-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.


# CODE
```
DEVELOPED BY:DIVYA K
REGISTER NUMBER:212222230035
```
```
import seaborn as sns
import pandas as pd
import matplotlib.pyplot as plt
df=sns.load_dataset('tips')
print(df)
df.isnull().sum()
plt.figure(figsize=(5,5))
plt.title("Data with outliers")
df.boxplot()
plt.show()
sns.barplot(x=df['day'],y=df['total_bill'],hue=df['day'])
plt.legend(loc='center')
plt.title("Highest Total Amount by the day of the week")
plt.show()
sns.boxplot(x=df['smoker'],y=df['tip'],hue=df['smoker'])
plt.title("Average tip amount given by smokers and non-smokers")
sns.boxplot(x='day',y='total_bill',hue='smoker',data=df,linewidth=2,width=0.6,boxprops={'facecolor':'lightblue','edgecolor':'darkblue'},whiskerprops={'color':'black','linestyle':"--","linewidth":1.5},capprops={'color':'black','linestyle':"--","linewidth":1.5})
df["tip_percent"]=df["tip"]/df["total_bill"]
sns.scatterplot(x=df['size'],y=df['tip_percent'],data=df)
plt.title("Tip Percentage by Dining Party Size")
sns.boxplot(x=df['sex'],y=df['tip'],hue=df['sex'])
plt.title("Tips based on gender")
sns.scatterplot(x=df['day'],y=df['total_bill'],hue=df['day'])
plt.legend(loc='best')
plt.title('Total bill amount by day of the week')
sns.histplot(data=df,x="total_bill",hue="time",element="step",stat="density")
plt.title("Distribution of Total Bill amounts by time of the day")
plt.show()
sns.boxplot(x="day",y="tip",data=df)
plt.title("Tip amount by day of the week")
plt.show()
sns.violinplot(x="time",y="tip",data=df)
plt.title("Tip amount by time of day")
plt.show()
sns.scatterplot(x="total_bill",y="tip",data=df)
plt.title("Correlation between tip amount and total bill amount")
plt.show()
```


# OUPUT
![282412986-e4d2f4c3-89d9-432e-8bfb-473937f27777](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/a3eebd36-3a3c-4626-974e-f17bb63952b6)




![282414307-2269fca5-da04-4ba0-b863-1e9792703a6d](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/1002dd2c-0629-461b-a146-b8d29398e26a)


![282414480-96f0eddf-02c8-46fc-b0cb-7b7002a1ca6f](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/62a488c4-6039-486e-83c2-63db18649534)


![282414651-26de21b5-065d-41a3-87b2-77a7707131ba](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/7cb1b5f2-7da5-4bdc-9a77-e8d5eb092889)



![282414742-5232d74a-0190-41ea-9d29-15e64616bcc7](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/4ec5c468-0ecb-4380-af26-3cbe6eeaa553)



![282414926-f09d0f86-f064-4977-a49d-2dc49608621c](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/efa9219f-45cb-4bc7-a2c0-77ec2f0584f1)



![282415004-7d3efe53-692f-4c6a-be37-93a445759f0e](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/4358ede8-bfa3-4ac2-9e64-dcca15cc0b76)





![282415100-8baec03c-7944-495b-8a92-b3d67bd16bd2](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/8c7668d1-b81e-498c-bc7d-908b5fe7448d)



![282415177-55741cc8-49a9-42a7-9910-bd5fc9b8978e](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/c3a21a4f-7389-45e4-a51a-67583bd5ce10)



![282415258-0b362a50-379a-49c1-a1e4-bea4eae64d6c](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/13403ab7-4873-4c5b-9c84-0c144731e117)




![282415331-7eab024c-db9e-4f3e-b71d-03427801d9af](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/1a705159-197d-406b-8c1d-b376a39871d6)



![282415435-7e1a3b90-41a0-4ffb-926e-d3164a81d76d](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/3f6d50d1-3403-4f0c-93f0-1d5c61bcc820)




![282415528-3f004468-6e15-4ac9-b999-72988138997e](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/f1b781a5-4938-4898-b127-df6a6eef9f71)



![282415682-5e41c8a8-296a-4a29-a6be-dbf944efd0e8](https://github.com/divyakumars/ODD2023-Datascience-Ex-09/assets/119393621/897a5923-b0ba-41dc-88a5-d8b6ed8288a2)
















# RESULT:
hus,data visulaization on a complex dataset is successfully executed.
