# Stroke Data Analysis | Streamlit & Google BigQuery

**Data Analytics Project | Python | Streamlit | Google BigQuery | Plotly | SQL**

## Project Overview

This project focuses on analysing stroke-related health, demographic, and lifestyle factors using an interactive multipage Streamlit application connected to Google BigQuery.

The objective is to explore patterns associated with stroke occurrence and provide interactive visualisations that help users understand relationships between age, gender, hypertension, heart disease, BMI, glucose levels, and lifestyle factors.

The project demonstrates practical skills in data analytics, cloud database integration, Python programming, and interactive dashboard development.

## Project Objectives

- Analyse demographic, health, and lifestyle factors associated with stroke occurrence.
- Clean and prepare healthcare data for analysis.
- Integrate Google BigQuery with a Python Streamlit application.
- Develop interactive visualisations using Plotly.
- Allow users to explore data using filters and sliders.
- Identify patterns and correlations between health indicators and stroke occurrence.

## Tools and Technologies

| Technology | Purpose |
|---|---|
| Python | Data processing and application development |
| Streamlit | Interactive multipage web application |
| Google BigQuery | Cloud data storage and SQL querying |
| SQL | Retrieving healthcare data |
| Pandas | Data cleaning and manipulation |
| Plotly Express | Interactive charts and visualisations |

## Dataset Description

The project uses a healthcare stroke dataset sourced from Kaggle.

The original dataset contains **5,110 records and 12 columns**. After removing records with missing BMI values, **4,909 records** remained for analysis.

The dataset includes:

- **Demographics:** Age, gender, marital status, and residence type.
- **Health Indicators:** Hypertension, heart disease, average glucose level, and BMI.
- **Lifestyle Factors:** Smoking status and work type.
- **Target Variable:** Stroke occurrence (`0 = No Stroke`, `1 = Stroke`).

## Application Architecture

```text
Healthcare Stroke Dataset
           |
           v
     Google BigQuery
           |
           v
      SQL Query
           |
           v
    Python & Pandas
     Data Cleaning
           |
           v
   Streamlit Application
           |
           v
  Interactive Visualisations
       Using Plotly
           |
           v
    Stroke Risk Factor
        Analysis
```

## Streamlit Application Features

The application contains seven pages:

| Page | Functionality |
|---|---|
| Home | Introduction and application overview |
| Dataset Overview | Total records, average age, median age, and stroke distribution |
| Gender Analysis | Gender distribution and stroke occurrence comparisons |
| Age Analysis | Age distributions, histograms, and stroke occurrence by age group |
| Health Factors Analysis | Hypertension and heart disease analysis |
| Lifestyle Factors Analysis | BMI, glucose levels, smoking status, and work type |
| Correlation Analysis | Scatter plots, correlation coefficients, and correlation heatmaps |

### Interactive Filters

Users can explore the dataset using:

- Gender selection dropdown.
- Age range slider.
- BMI range slider.
- Work type text input.
- Stroke occurrence filter.

The visualisations update dynamically based on the selected filters.

## Key Findings

The analysis identified several patterns associated with stroke occurrence.

| Factor | Finding |
|---|---|
| Age | Stroke cases were more common among older individuals, particularly those aged 60 and above |
| Gender | Approximately 59% of the analysed records were female and 41% male |
| Hypertension | 12.8% of individuals with hypertension had experienced a stroke |
| Heart Disease | 15.3% of individuals with heart disease had experienced a stroke |
| BMI and Glucose | The application explored their distributions and relationships with stroke occurrence |

These findings describe patterns in the dataset and do not establish causation or provide an independently validated clinical risk prediction model.

## Project Repository Structure

All files are stored directly in the main GitHub repository.

```text
stroke-data-analysis-streamlit/
│
├── README.md
├── 1. Project Description.pdf
├── 2. RAW-data-healthcare-dataset-stroke.csv
├── 3. Report.pdf
├── 4. Final code.txt
├── 5. Code explanation.docx
└── 6. Presentation.pptx
```

## Project Files

| File | Description |
|---|---|
| `1. Project Description.pdf` | Project requirements and objectives |
| `2. RAW-data-healthcare-dataset-stroke.csv` | Original healthcare stroke dataset |
| `3. Report.pdf` | Detailed analysis, application screenshots, and findings |
| `4. Final code.txt` | Python source code for the Streamlit application |
| `5. Code explanation.docx` | Explanation of the code and application functionality |
| `6. Presentation.pptx` | Project presentation and visualisations |

## How to Run the Project

**Prerequisites:** Python, Streamlit, Pandas, Plotly, and Google Cloud BigQuery access.

1. Clone or download the repository.
2. Install the required Python libraries:

```bash
pip install streamlit pandas plotly google-cloud-bigquery db-dtypes matplotlib seaborn
```

3. Configure Google Cloud credentials with access to the BigQuery dataset.
4. Update the local credentials path in the source code.
5. Rename `4. Final code.txt` to `app.py`.
6. Run the application:

```bash
streamlit run app.py
```

**Note:** The application requires access to the Google BigQuery table `bia712-assignment.StrokePrediction.StrokePredictionTable`. The CSV file alone is not sufficient to run the current code without modifying the data-loading logic. Never commit Google Cloud service account credentials to a public repository.

## Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- SQL and Google BigQuery
- Cloud Database Integration
- Streamlit Application Development
- Interactive Data Visualisation
- Statistical and Correlation Analysis
- Data-Driven Reporting

## Conclusion

This project demonstrates how Python, Streamlit, Google BigQuery, and Plotly can be combined to develop an interactive healthcare analytics application.

By analysing demographic, health, and lifestyle factors, the application provides an accessible way to explore stroke occurrence patterns and supports data-driven research.

## Author

**Yolisa Velebayi**

Data Analytics | Data Engineering | Business Intelligence

**GitHub:** [github.com/Yolisa95](https://github.com/Yolisa95)

---

*Part of my data analytics portfolio showcasing Python, cloud data integration, interactive dashboards, and healthcare data analysis.*
