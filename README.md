# udemy-data-analysis
This repository contains a Udemy Course Data Analysis project, focusing on data cleaning, exploratory data analysis (EDA), and visualization. Using Python libraries like Pandas, Matplotlib, and Seaborn
# 📊 Data Analysis | Udemy Data Analysis

## 📌 Project Overview  
This project analyzes Udemy's course dataset to uncover **trends in course popularity, pricing, ratings, and instructor impact**. The goal is to provide insights into what makes courses successful and identify key patterns in online learning.  

## 🔍 Key Features  
✔️ **Cleaned & pre-processed the dataset** to ensure accuracy and consistency.  
✔️ **Performed Exploratory Data Analysis (EDA)** to discover trends in course popularity, pricing, and instructor success.  
✔️ **Created data visualizations** using **Matplotlib & Seaborn** to represent insights clearly.  
✔️ **Answered business-driven questions**, such as:  
   - What are the most popular course categories?  
   - How does pricing affect enrollment?  
   - Do higher-rated courses have more students?  

## 🛠️ Technologies Used  
- **Python**  
- **Pandas** (for data manipulation)  
- **Matplotlib & Seaborn** (for visualization)  
- **NumPy**  
- **Jupyter Notebook**  

## 📊 Sample Analysis  
### 🔹 Most Popular Course Categories  
```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Load dataset
df = pd.read_csv("udemy_data.csv")

# Count course categories
category_counts = df['category'].value_counts().head(10)

# Plot top categories
plt.figure(figsize=(10,5))
sns.barplot(x=category_counts.index, y=category_counts.values, palette="coolwarm")
plt.title("Top 10 Most Popular Course Categories on Udemy")
plt.xlabel("Category")
plt.ylabel("Number of Courses")
plt.xticks(rotation=45)
plt.show()

```
<hr>
<p align="center">
  <img src="Udemy.png" alt="Udemy" width="800">
</p>




