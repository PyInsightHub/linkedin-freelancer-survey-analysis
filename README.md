# LinkedIn Freelancer Survey Analysis

Exploratory data analysis of LinkedIn freelancer survey results, built with Python, Pandas, Matplotlib, Seaborn and Plotly.

## Overview

This project analyzes aggregated responses to a 50-question multiple-choice survey. For each question, the dataset records the share of respondents who chose each option (A, B, C, D) and the number of respondents. The analysis covers data validation, response distributions, average response proportions, and the relationship between response patterns and sample size.

## Dataset

**File:** `data/results.csv`

| Column | Description |
|---|---|
| `question` | Survey question number (1-50) |
| `A`, `B`, `C`, `D` | Proportion of respondents who selected each option |
| `respondents` | Number of respondents for that question |

**Dataset summary**
- 50 rows (one per question), 6 columns
- No missing values
- Response proportions sum to approximately 1.0 for every question
- Respondents per question range from 6 to 478 (average of about 72)

## Methodology

1. **Data Import:** load the dataset and inspect its structure
2. **Data Cleaning:** check for duplicates, missing values, negative values and data types
3. **Exploratory Data Analysis:** visualize response distributions across all questions
4. **Response Proportion Analysis:** compare average proportions for each option
5. **Correlation Analysis:** examine relationships between response proportions and respondent counts

## Key Visualizations

- Response distribution across survey questions (line charts, static and interactive)
- Number of respondents per question
- Stacked bar chart of response composition by question
- Average response proportion by category
- Box plot of response proportion distributions
- Correlation matrix

## Key Observations

- Option **B** was the most-chosen answer on 19 of the 50 questions, followed by **A** (15), **C** (11) and **D** (5).
- Sample sizes vary widely, so questions with very few respondents (for example, questions 1-5) produce less reliable percentages.

## Tech Stack

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Plotly
- Jupyter Notebook / Google Colab

## Repository Structure

```
linkedin-freelancer-survey-analysis/
│
├── data/
│   └── results.csv
├── linkedin_freelancer_survey_analysis.ipynb
├── requirements.txt
└── README.md
```

## Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/your-username/linkedin-freelancer-survey-analysis.git
cd linkedin-freelancer-survey-analysis
```

**2. Install dependencies**
```bash
pip install numpy pandas matplotlib seaborn plotly jupyter
```

**3. Launch the notebook**
```bash
jupyter notebook linkedin_freelancer_survey_analysis.ipynb
```

> **Note:** Update the data path in the notebook to `data/results.csv` if you are running it locally.

## Future Improvements

- Add statistical significance testing across response options
- Weight results by respondent count
- Build an interactive dashboard (Streamlit or Power BI)

## Author

**Arpan Ghosal**
[LinkedIn](https://www.linkedin.com/in/arpan-ghosal-15a430338/) | [GitHub](https://github.com/PyInsightHub)
