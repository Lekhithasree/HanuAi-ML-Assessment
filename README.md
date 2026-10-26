
# HanuAi ML Assessment

## Project Overview

This project is developed as part of the HanuAi Machine Learning Assessment.

The objective is to apply Python, Machine Learning, Natural Language Processing (NLP), and Data Analytics to extract meaningful insights from customer reviews and technical complaint data.

The assessment consists of two tasks:

1. Web Scraping and Sentiment Analysis
2. Advanced Exploratory Data Analysis (EDA) and Text Mining

## Task 1: Web Scraping and Sentiment Analysis

Status: Planned

### Objective
Collect publicly available product reviews from Best Buy Canada, analyze customer sentiment, and identify satisfaction and dissatisfaction drivers.

### Planned Implementation
- Select a product with at least 50 reviews.
- Extract review details using Python browser automation and HTML parsing.
- Handle review pagination and sorting filters.
- Collect review titles, text, dates, ratings, sources, and reviewer names.
- Classify reviews as Positive, Negative, or Neutral.
- Generate aspect-based sentiment tags.
- Document responsible approaches to scraping challenges.
- Provide actionable customer satisfaction insights.

## Task 2: Advanced EDA and Text Mining

Status: In Progress

### Objective
Analyze vehicle-related customer complaints to identify recurring issues, extract structured information, detect patterns, and investigate potential causes of failures.

### Dataset
- Source: HanuAi assessment dataset
- Format: CSV
- Records: 1,000
- Original columns: 20

The dataset contains customer complaints, technician diagnoses, repair descriptions, vehicle information, and technical failure categories.

The original assessment dataset is excluded from this public repository.

### Implemented Work

#### 1. Data Understanding and Cleaning
- Examined dataset structure and data types.
- Identified missing values.
- Applied column-specific missing-value handling.
- Checked duplicate records.
- Standardized date columns.
- Identified important stakeholder-related features.

#### 2. Exploratory Data Analysis
- Calculated descriptive statistics.
- Analyzed complaints by vehicle make and model.
- Analyzed monthly complaint trends.
- Examined customer complaint categories.
- Examined recorded technical failure causes.
- Analyzed complaint distribution by manufacturing plant.
- Created visualizations using Matplotlib.

#### 3. Text Preprocessing
- Identified customer complaint, technician diagnosis, and repair description fields.
- Normalized text formatting and whitespace.
- Preserved technical terminology and diagnostic codes.
- Retained original text for traceability.

#### 4. NLP Entity Extraction
Implemented initial rule-based entity extraction using Python regular expressions.

Target entities include:
- Components: Radio, Display, Camera, Amplifier, Battery
- Symptoms: Black Screen, No Audio, Intermittent Failure
- Diagnostic Trouble Codes: Recognized automotive error-code patterns

### Remaining Work
- Validate extracted NLP entities.
- Improve entity extraction coverage.
- Classify complaints into higher-level issue categories.
- Apply TF-IDF and unsupervised clustering.
- Analyze recurring failure patterns and potential root causes.
- Develop actionable stakeholder recommendations.
- Export the enriched dataset.
- Prepare the final stakeholder report.

## Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Regular Expressions (Regex)
- Visual Studio Code
- Git and GitHub

## Project Structure

```text
HanuAi-ML-Assessment/
├── task2_eda_text_mining.ipynb
├── README.md
└── .gitignore
```

Additional notebooks, reports, and permitted outputs will be added as the project progresses.

## Running the Project

1. Clone the GitHub repository.
2. Create a Python virtual environment.
3. Activate the environment.
4. Install the required Python libraries.
5. Obtain the original Task 2 dataset through an authorized source.
6. Place the dataset in the project directory.
7. Open the Jupyter Notebook in VS Code.
8. Select the project Python environment.
9. Run the notebook cells sequentially.

Required Python libraries for the current notebook:

```bash
python -m pip install pandas numpy matplotlib seaborn scikit-learn ipykernel openpyxl
```

Note: The assessment dataset is not included in the public repository, so data-dependent analyses require authorized access to that file.

## Business Value

The project aims to support:
- Identification of frequently reported technical issues.
- Analysis of customer complaint trends.
- Recognition of recurring failure patterns.
- Investigation of potential component-related problems.
- Data-driven quality improvement recommendations.

Complaint counts represent the supplied records and should not be interpreted as failure rates without relevant vehicle population data.

## Current Status

Task 2 EDA and initial rule-based NLP entity extraction have been implemented. Validation, clustering, and reporting remain in progress.

Task 1 implementation has not yet started.

The repository will be updated as additional assessment requirements are completed.
