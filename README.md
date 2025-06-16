# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

📌 Project Overview

This project investigates an insurance dataset to understand the key factors that influence medical insurance charges. The dataset includes variables such as age, sex, BMI, smoking status, and region. Using Python in Jupyter Notebook, I conducted a detailed exploratory data analysis (EDA) to explore correlations, uncover patterns, and visualise the relationships between these variables. The aim was to draw meaningful insights that could inform decision-making in pricing strategies or risk modelling in the insurance industry. The analysis combines statistical techniques and visual storytelling through a range of plots and a correlation heatmap.

🧼 Data Cleaning

Before the analysis could begin, the original dataset required significant cleaning and restructuring. This involved:

* Handling missing values

* Converting categorical variables into appropriate formats

* Ensuring numerical data consistency and accuracy

All cleaning was performed using Python scripts via the terminal. The cleaned dataset was saved as cleaned_insurance.csv and stored in a structured data/ folder. This ensured a reproducible and well-organised workflow, ready for analysis.

📊 Visualisations Conducted

✅ Scatter Plot

* Insurance charges vs. age, colour-coded by smoking status

✅ Box Plot

* Distribution of insurance charges across genders

✅ Bar Chart

* Comparison of average insurance charges between smokers and non-smokers

✅ Heatmap

* Correlation matrix showing relationships among all numerical features

These visualisations helped to highlight key trends and provide an intuitive understanding of the data distribution and relationships.

💡 Insights and Findings
* Smoking is the most significant contributor to higher insurance charges

* Insurance costs increase with age, particularly for smokers

* Gender shows visible distribution differences, but its direct impact is less significant than smoking or BMI

* The heatmap revealed strong positive correlations between smoking, BMI, and charges

These insights demonstrate how lifestyle and demographic factors play a crucial role in insurance pricing.

🚧 Challenges and Solutions

📁 FileNotFoundError and Path Confusion

When attempting to run all cells in the Jupyter Notebook, inconsistent file path errors (FileNotFoundError) would occur. This was due to how the notebook was launched and how relative paths were resolved.

✅ Solution:
I used Python’s os module to check and manually set the working directory:

import os  
os.chdir('/Users/nasraibrahim/Documents/vscode-projects')

This ensured that the correct directory structure was recognised regardless of how the notebook was opened or run, allowing the data file to be located consistently.

🧼 Data Cleaning and Preparation

The dataset required extensive cleaning, including handling missing values, correcting data types, and encoding categorical variables. Executing this in the terminal using Python was often slow and error-prone.

✅ Solution:

I used an iterative approach — checking data structure with .info() and .columns, converting data types using .astype() and pd.to_numeric(), and testing changes step-by-step to avoid further errors. This process ensured the cleaned dataset was accurate and ready for analysis.

📊 Plotly and Visualisation Issues

While working with Plotly for interactive visualisations, I encountered rendering problems, particularly when moving from Jupyter to GitHub, where interactive charts were not supported.

✅ Solution:

I resolved this by installing and configuring kaleido to export Plotly visuals as static .png files, which allowed them to be displayed correctly on GitHub. This adjustment maintained the quality of the visual output across platforms.

⚙️ Virtual Environment and Package Installation

Setting up the .venv environment and installing necessary packages such as nbformat, ipykernel, and kaleido led to multiple dependency conflicts and installation errors.

✅ Solution:

By carefully managing the virtual environment, reinstalling problematic packages, and consulting documentation and AI tools, I was able to stabilise the environment. This allowed for seamless notebook execution, data cleaning, and visual exports.

🤖 Tools That Helped

To overcome these challenges, I made extensive use of ChatGPT and GitHub Copilot. These tools offered real-time support in debugging, writing clean code, resolving path issues, and adjusting visualisation outputs. With their help, I was able to build a consistent, reproducible workflow that could run smoothly both locally and on GitHub.

📈 Conclusion and Next Steps

This project demonstrates the value of exploratory data analysis in revealing patterns and relationships within structured datasets. It also highlights the importance of clean project organisation and environment setup to ensure reliable and reproducible work.

Potential next steps include:

* Building predictive models to estimate charges based on input features

* Applying regression analysis or machine learning techniques

* Conducting hypothesis testing for deeper statistical insight

* Further feature engineering and data enrichment to improve model performance

📚 References

Kaggle: Insurance Dataset

ChatGPT (OpenAI) — for coding support, debugging, and structural guidance

GitHub Copilot — for auto-completion and efficient script writing

pandas Documentation — for data cleaning and manipulation

matplotlib & seaborn — for creating professional visualisations