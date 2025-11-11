# Mental Health in the Tech Industry: A Demographic Analysis
## Project Overview
This notebook examines mental health data within the tech industry, focusing on the relationship between mental illness reporting rates and demographic factors such as age, gender, and race. Drawing on survey data from tech employees, this analysis contrasts these findings with national averages from the National Institute of Mental Health (NIMH) to understand how mental health is experienced and reported in this specific workforce.

## Dataset
The dataset used in this project is titled Mental Health in the Tech Industry and is sourced from Kaggle. The data file (mental_health.sqlite) is available within this repository.

- File Format: SQLite database (mental_health.sqlite)
- Source: [Mental Health in Tech Survey on Kaggle](https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry)
- Description: This dataset contains responses from employees in the tech industry regarding their mental health, including questions about demographic details, mental health status, and comfort discussing mental health issues in the workplace.

## Installation
This project requires several Python libraries to run the data analysis and visualizations. You can install the necessary packages using the commands below.

1. Clone the repository or download the files.
2. Create and activate a virtual environment (optional but recommended):

```bash
   python -m venv env
   source env/bin/activate  # On macOS and Linux
   .\env\Scripts\activate   # On Windows
```

3. Install the required packages:

```bash
pip install pandas sqlite3 seaborn numpy matplotlib requests scipy statsmodels datasets
```

Package Details:
- pandas: For data manipulation and analysis.
- sqlite3: To connect and query data from a SQLite database.
- seaborn: For creating attractive data visualizations.
- numpy: For numerical operations.
- matplotlib: For data visualization and customization.
- requests: For handling HTTP requests (e.g., to fetch external datasets if needed).
- datasets: A library by Hugging Face to load and manage datasets.
- scipy: For statistical functions.
- statsmodels: For statistical modeling and confidence interval calculations.
- If you encounter any installation issues, ensure that you have an updated version of pip:

```bash
pip install --upgrade pip
```

## Usage
Once the dependencies are installed, you can run the analysis and visualizations by opening the project in Jupyter Notebook or directly in VS Code (if using Jupyter extension) and following along with the notebook cells.

## Data and Methodology
The dataset analyzed in this project includes survey responses collected across multiple years. The data comprises the following key columns:

- SurveyID (corresponding to survey year)
- UserID (unique identifier for each respondent)
- AnswerText (respondent's answer text)
- QuestionText (survey question)
- QuestionID (corresponding to specific survey questions)

To examine the trends over time, the analysis focused on self-reported mental health conditions as well as respondents' comfort in discussing mental health issues with their supervisors.

## Key Findings
1. Gender and Racial Disparities in Mental Illness Reporting
Male respondents and white respondents reported mental illness at rates aligning more closely with the national averages than female respondents and racial minorities, whose rates appeared significantly lower than NIMH's reported national averages.
These differences suggest potential barriers in mental health reporting among female and racial minority respondents within tech, possibly due to privacy concerns or fear of workplace repercussions.
2. Comfort Discussing Mental Health with Supervisors
Although a visual representation could not be generated for yearly gender-based comfort levels in discussing mental health issues with supervisors, this information is available as a DataFrame within the project.
Notably, in 2019, there was a significant increase in female respondents who reported they would not feel comfortable discussing mental health issues with their supervisors, coinciding with heightened anxiety around societal events, such as the lead-up to the 2020 U.S. election.
3. Reporting Anomalies in 2019
In 2019, both the percentage of respondents choosing not to identify their race and the number of female respondents uncomfortable discussing mental health with supervisors spiked. This could reflect heightened privacy concerns or workplace anxieties within the tech industry, potentially tied to broader societal tensions at that time.
4. Interpretation of Reporting Discrepancies
One possible explanation for the discrepancy between NIMH data and tech survey data is the lack of comfort among female and racial minority respondents in disclosing mental health concerns in a workplace-connected survey. This suggests that these groups may avoid reporting mental health challenges in professional contexts due to concerns about privacy or career impact.

## Recommendations for Tech Companies
To create a supportive work environment that encourages open mental health discussions, tech companies should consider the following actions:

1. Address Unhealthy Work Culture
Employees should not feel pressured to overwork, whether directly or indirectly. Companies need to foster balanced workloads and encourage a culture where taking time off for mental health is normalized.

2. Promote Equity and Career Advancement
Establishing fair opportunities for growth can reduce the apprehension among women and racial minorities about reporting mental health issues. Mentorship programs can be a powerful tool to foster talent and ensure individuals feel supported and valued, regardless of demographic background.

3. Build Trust in Privacy and Anonymity
Clear and consistent communication regarding the anonymity of feedback and surveys is crucial. Companies should work to instill trust in the confidentiality of employees’ responses by reducing office gossip and offering anonymous feedback options more regularly.

4. Engage Employees in Workplace Improvements
Incorporating employee feedback into decision-making fosters buy-in and ensures that changes align with employees’ genuine needs. Engaging teams in conversations about mental health and workplace culture can create a more supportive environment tailored to employees' real concerns.

## Conclusion
Thank you for reviewing this analysis. The findings underscore the need for tech companies to create environments where employees feel safe discussing mental health. Addressing work culture, ensuring equitable opportunities, respecting privacy, and engaging employees in shaping workplace dynamics can lead to a more supportive, inclusive environment for all.
