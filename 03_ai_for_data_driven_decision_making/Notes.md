# Data Cleaning Checklist
1. Initial Data Inspection
    - Data used: ![alt text](data_cleaning.csv)
    - Prompt:
    <blockquote>
    I have uploaded a dataset of sales. Can you provide me a comprehensive overview of the data? 
    1. The number of rows and columns
    2. Datatype of each column
    3. Basic statistical summary of each column (include mean, median, standard deviation, min, max, quantiles) for numerical columns
    4. Number of unique values, and most occurring values for each of the text and categorical columns
    5. Any obvious errors, missing values, inconsistencies and potential data quality concerns

    Explain your findings in concise and clear manner
    </blockquote>

2. Handling Missing Values
    - Prompt:
    > For the missing values in the 'Total Sales' column of the attached dataset, can you suggest an appropriate imputation method using other relevant columns to predict the missing income? Explain your approach, suggest a prompt to implement it, and provide the reasoning behind your choice.

3. Standardizing Formats
    - What to consider: Dates, Numbers (inconsistent decimal separators), Currencies, Text (inconsistent capitalization, extra spaces, special characters), Categorical Data (Inconsistent category names)
    - Prompt:
    > Convert all dates in the Dates to the ISO 8601 format (YYYY-MM-DD). Handle any variations in date formats that might be present.

4. Handling Duplicate Entries
    - Identify and address duplicate rows, considering whether they are errors or meaningful data points.
    - Prompt:
    > "Identify and remove any duplicate rows from the dataset. Base the identification of duplicates solely on the 'Order ID' column. Keep the first occurrence of each unique Order ID.


5. Data Cleaning Log
Crucially, create a separate document (or a section within your analysis document) to record all data cleaning steps taken. This is essential for reproducibility and transparency. Include:
- Date of cleaning.
- Description of each cleaning step (e.g., "Removed rows with missing values in 'Order ID' column").
- The rationale for each step (e.g., "Missing Order IDs would prevent accurate
order tracking").
- The AI prompt used (if applicable).
- The number of rows/values affected (e.g., "5 rows removed")    


# AI powered Data analysis (EDA)
- Initial Data Overview: Start with a dataset description (rows, columns, data types) and missing value analysis to understand structure and quality, using prompts like "Describe the dataset" or "Identify missing values."
- Statistical Insights: Generate descriptive statistics (mean, median, etc.) for numerical columns and unique value counts for categorical/text columns to grasp distributions and identify anomalies, with prompts like "Generate descriptive statistics" or "Report unique values."
- Relationship Exploration: Analyze time series trends, correlations between numerical variables, and group comparisons (e.g., sales by category) using prompts like "Analyze trends" or "Compare average sales," supported by charts and tests.
Anomaly Detection: Identify outliers in numerical data (via IQR method) and unusual text entries to ensure data integrity, with prompts like "Identify outliers" or "Examine text anomalies."
- Hypothesis and Preparation: Generate testable hypotheses from insights and assess feature importance for machine learning, using prompts like "Generate hypotheses" or "Identify important predictors," while documenting findings.


# Visual Storytelling
- Pre-Story Foundation: Identify 2-3 key data insights, define your audience (e.g., executives, marketers) with their knowledge level and concerns, set a clear desired outcome (e.g., budget approval), and choose a narrative angle (e.g., problem/solution).
- Crafting Narratives with AI: Use tailored ChatGPT prompts (e.g., executive summary, marketing narrative) with the PROMPT framework (Purpose, Role, Output, Markers, Patterns, Tone) to create targeted, concise stories (150-200 words) for specific audiences.
- Selecting Impactful Visuals: Leverage AI to recommend chart types (e.g., line chart for trends, bar chart for comparisons) based on data type and audience, ensuring visuals enhance the narrative with clear features like trendlines.
- Presentation Checklist: Ensure audience alignment, clarity, effective visuals, ethical accuracy/transparency, and a SMART call to action, followed by practice and feedback.
- Key Principles: Start with "why," iterate AI responses, use human judgment, simplify language, and make the story memorable with visuals, analogies, and examples.

