# CodeAlpha Internship Task 2: Exploratory Data Analysis (EDA)

This repository contains the complete Exploratory Data Analysis (EDA) of the `user_level_ai_adoption.csv` dataset, completed as part of the CodeAlpha Data Science Internship. The analysis is structured to be simple, beginner-friendly, and interview-ready.

---

## 📌 Project Overview
The goal of this project is to perform a thorough, manual-style Exploratory Data Analysis to identify trends, patterns, and insights in user-level AI tool adoption. We look at user profiles (industry, role, location, experience) and metrics of tool utilization (daily token usage, automated tasks) to understand their combined impact on productivity gains.

## 📊 Dataset Description
The dataset contains **15,000 records** and **10 columns**:
- `User_ID`: Unique user identifier (String)
- `Industry`: Industry sector of the user (Categorical)
- `Job_Role`: Job role of the user (Categorical)
- `Location`: Geographic region (Categorical)
- `Experience_Years`: Professional work experience in years (Numerical)
- `Primary_AI_Tool`: The primary AI tool used by the user (Categorical)
- `Daily_Token_Usage`: Number of AI tokens consumed daily (Numerical)
- `Tasks_Automated_Per_Week`: Number of tasks automated weekly (Numerical)
- `Productivity_Gain_Percent`: Productivity gain reported (Numerical)
- `Adoption_Date`: Date of AI tool adoption (Datetime)

## 🛠️ Libraries Used
The project is built entirely on standard, beginner-friendly Python data science libraries:
- `pandas` for data loading, inspections, and cleanups.
- `numpy` for basic descriptive statistical calculations.
- `matplotlib.pyplot` for creating plot canvases and customizing axes.
- `seaborn` for clean statistical visualizations.

## 📂 Project Structure
The repository follows a clean, minimal folder structure:
- `user_level_ai_adoption.csv` : The raw dataset.
- `CodeAlpha_EDA.ipynb` : The main Jupyter Notebook containing all 27 sections of the EDA, code blocks, executed outputs, and simple observations.
- `requirements.txt` : List of Python dependencies.
- `.gitignore` : Git ignore configurations.
- `README.md` : Detailed project report and guide.

---

## 📈 EDA Steps Completed
1. **Project Introduction & Setup**
2. **Data Inspection**: Displaying head, tail, sample, shape, column names, and datatypes.
3. **Data Quality Audit**: Explicit checking for missing values, duplicates, and unique categorical values.
4. **Descriptive Statistics**: Calculated mean, median, mode, minimum, maximum, standard deviation, quartiles, IQR, skewness, and kurtosis.
5. **Univariate Analysis**: Histograms, KDE, and boxplots for numerical columns; count plots and pie charts for categorical features.
6. **Bivariate Analysis**: Scatter plots, grouped bar charts, and category-level boxplots.
7. **Correlation Analysis**: Correlation matrix heatmap.
8. **Outlier Detection**: Using IQR bounds to identify extreme productivity gains.
9. **Trend and Hypothesis Testing**: Line charts for monthly adoption and checking two simple hypotheses.
10. **Final Insights**: Summarizing takeaways, business value, data limitations, and recommendations.

---

## 💡 Key Findings
1. **Career Tenure Neutrality (The Great Equalizer)**:
   The correlation between `Experience_Years` and `Productivity_Gain_Percent` is virtually **0.00**. Junior, mid-level, and senior professionals all achieve an average productivity gain of **~11.2%**, showing that AI adoption benefits users equally across all tenure levels.
2. **Non-linear Automation Payoff**:
   We checked the hypothesis *"More tasks automated leads to higher productivity gains"* (Correlation: **0.70**). While passthrough token usage yields modest gains, once a user automates **more than 14 tasks per week**, their productivity gain spikes exponentially up to **84.9%**.
3. **Industry Tooling Alignment**:
   Specialized AI tools follow industrial patterns: **GitHub Copilot** is heavily concentrated in *Software Development*, while **Midjourney** is dominant in *Creative & Design*. General-purpose assistants (ChatGPT, Claude) are adopted broadly across all sectors.
4. **Strong Utilization Coupling**:
   `Daily_Token_Usage` and `Tasks_Automated_Per_Week` have a strong positive correlation of **0.82**, confirming that active task automation is the primary driver of token consumption.

---

## 🚀 How to Run

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/vaibhav1874/CodeAlpha_Exploratory-Data-Analysis-EDA-.git
   ```
2. Navigate into the repository:
   ```bash
   cd CodeAlpha_Exploratory-Data-Analysis-EDA-
   ```
3. Install the required libraries using pip:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the Jupyter Notebook server:
   ```bash
   jupyter notebook
   ```
5. Click on `CodeAlpha_EDA.ipynb` and run the cells sequentially to reproduce the entire report.

---

## 🔮 Future Improvements
- **Feature Engineering**: Creating an automation efficiency score (`Tasks_Automated_Per_Week` / `Daily_Token_Usage`).
- **Additional Data**: Collecting data on training history and paid vs free subscription tiers to see if training increases adoption speeds.
- **Predictive Modeling**: Building a robust regression model to predict `Productivity_Gain_Percent` based on usage patterns.
