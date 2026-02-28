# task6

📊 Task 6: Correlation Heatmap

This project demonstrates how to create a Correlation Heatmap using Python libraries like Pandas, Seaborn, and Matplotlib.
A heatmap helps visualize the relationship between numerical variables in a dataset.

📁 Dataset

Dataset used: Students Performance Dataset
Source: Kaggle
Link: https://www.kaggle.com/datasets/spscientist/students-performance-in-exams

The dataset contains student scores in:

Math

Reading

Writing

🎯 Objective

The goal of this task is to:

Understand relationships between variables

Calculate correlation between features

Visualize correlations using a heatmap

🛠️ Technologies Used

Python

Pandas

Seaborn

Matplotlib

Jupyter Notebook / VS Code

📌 Steps Performed

Imported required libraries

Loaded the dataset

Selected numerical columns

Calculed correlation matrix

Plotted correlation heatmap using Seaborn

💻 Code Example
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv("StudentsPerformance.csv")

# Correlation matrix
corr = df.corr(numeric_only=True)

# Plot heatmap
plt.figure(figsize=(8,6))
sns.heatmap(corr, annot=True, cmap="coolwarm")

plt.title("Correlation Heatmap of Student Scores")
plt.show()
📈 Output

The heatmap shows correlation between:

Math Score

Reading Score

Writing Score

Darker colors represent stronger relationships between variables.

✅ Conclusion

Reading and Writing scores have strong correlation

Math score is moderately correlated with Reading and Writing

Heatmaps make data relationships easy to understand visually

📂 Project Structure
Task6-Heatmap/
│── StudentsPerformance.csv
│── heatmap.ipynb
│── README.md

🚀 Author

sk mahamood anzar
Data Science Intern – KodBud
