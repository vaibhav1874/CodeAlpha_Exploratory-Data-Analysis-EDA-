# CodeAlpha Task 2: Exploratory Data Analysis (EDA)

This is my project for Task 2 (Exploratory Data Analysis) of the CodeAlpha internship. 

I did an EDA on the `user_level_ai_adoption.csv` dataset to see how people use AI tools and how it affects their productivity.

## About the Dataset
The dataset contains 15,000 rows and 10 columns:
- `User_ID`: Unique user ID
- `Industry`: Industry sector (Software Development, Healthcare, etc.)
- `Job_Role`: Job role of the user (Data Analyst, Developer, etc.)
- `Location`: Geographic region (North America, Europe, etc.)
- `Experience_Years`: Years of work experience
- `Primary_AI_Tool`: The main AI tool used by the user
- `Daily_Token_Usage`: Number of AI tokens consumed daily
- `Tasks_Automated_Per_Week`: Weekly automated tasks
- `Productivity_Gain_Percent`: Productivity gain reported
- `Adoption_Date`: Date of AI tool adoption

## Libraries Used
I used standard python data science libraries:
- **Pandas** for loading and checking the data structure
- **NumPy** for descriptive stats
- **Matplotlib and Seaborn** for drawing distributions and trend charts

## Project Files
- `user_level_ai_adoption.csv` : Raw dataset
- `CodeAlpha_EDA.ipynb` : The main notebook containing the full analysis
- `requirements.txt` : Python requirements
- `.gitignore` : Ignore temp files
- `README.md` : Project documentation

## Key Findings
- **Equal Opportunity**: Experience years has almost 0 correlation with productivity gains. Juniors and seniors get similar productivity improvements.
- **Tipping Point**: Productivity gains rise exponentially once a user automates more than 14 tasks per week.
- **Tool Choices**: Midjourney is used in Creative & Design, GitHub Copilot is in Software Development. General-purpose tools (ChatGPT, Claude) are used across all industries.
- **Daily Usage**: Daily token usage is strongly correlated with weekly automated tasks (0.82), meaning active task automation is what drives token use.

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Start Jupyter:
   ```bash
   jupyter notebook
   ```
3. Open `CodeAlpha_EDA.ipynb` and run the cells.
