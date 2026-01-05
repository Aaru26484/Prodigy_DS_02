# 📊 Prodigy Infotech – Data Science Internship  
## Task 02: Data Cleaning & Exploratory Data Analysis (EDA)

### 👤 Intern
**Aarti Singh**

---

## 📌 Task Description
The objective of this task is to perform **data cleaning** and **exploratory data analysis (EDA)**
on a dataset in order to understand its structure, explore relationships between variables,
and extract meaningful insights before applying machine learning techniques.

---

## 🎯 Objectives
- Clean and preprocess the dataset  
- Handle missing and inconsistent values  
- Analyze numerical features  
- Identify correlations between variables  
- Visualize data using plots and heatmaps  

---

## 📂 Dataset
- **Dataset Used:** Titanic Dataset  
- The dataset contains passenger information such as age, fare, class, and survival status.

---

## 🛠️ Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Google Colab / Jupyter Notebook  

---

## 🔍 Exploratory Data Analysis
The following steps were performed:
1. Data loading and inspection  
2. Handling missing values  
3. Selection of numerical features  
4. Correlation analysis  
5. Visualization using a correlation heatmap  

---

## 📈 Correlation Heatmap
The correlation heatmap below visualizes relationships between numerical features in the dataset:

```python
plt.figure(figsize=(8,6))

numeric_df = df.select_dtypes(include=['int64', 'float64'])
sns.heatmap(numeric_df.corr(), annot=True, cmap='coolwarm')

plt.title("Correlation Heatmap (Numeric Features)")
plt.show()
