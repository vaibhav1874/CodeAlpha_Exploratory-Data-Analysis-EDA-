# CodeAlpha Task 2: Exploratory Data Analysis (EDA)

This project contains the Exploratory Data Analysis (EDA) on `user_level_ai_adoption.csv` dataset, completed as part of the CodeAlpha Data Science Internship.

## Project Overview
The goal of this analysis is to explore a dataset representing user-level AI tool adoption across various industries, regions, and experience levels. We investigate what factors drive productivity gains, daily token usage, and automation levels, and identify patterns and outliers.

## Dataset Description
The dataset `user_level_ai_adoption.csv` contains 15,000 records and 10 features:
- `User_ID`: Unique user identifier
- `Industry`: Industry sector of the user
- `Job_Role`: Job role of the user
- `Location`: Geographic region
- `Experience_Years`: Professional work experience (in years)
- `Primary_AI_Tool`: The primary AI tool used by the user
- `Daily_Token_Usage`: Number of AI tokens consumed daily
- `Tasks_Automated_Per_Week`: Weekly automated tasks
- `Productivity_Gain_Percent`: Percent productivity gain reported
- `Adoption_Date`: Date of AI tool adoption

## Libraries Used
- **Pandas**: For data loading, manipulation, and structural understanding.
- **NumPy**: For statistical analysis and data operations.
- **Matplotlib**: For basic plotting and customization.
- **Seaborn**: For statistical data visualization.

## Project Structure
- `user_level_ai_adoption.csv` : Raw dataset
- `CodeAlpha_EDA.ipynb` : Jupyter Notebook containing the entire step-by-step EDA
- `requirements.txt` : Python package requirements
- `.gitignore` : Git ignore configurations
- `README.md` : Project documentation

## How to Run
1. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
2. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open `CodeAlpha_EDA.ipynb` and run the cells.
