**Impact of Length of Stay on Mental Health Outcomes Among International Students (SQL Analysis)**

This project explores whether the length of stay in a foreign country influences the mental health outcomes of international students. Using real survey data collected by a Japanese international university in 2018, the analysis evaluates diagnostic test scores related to:

Depression (PHQ-9)

Social Connectedness (SCS)

Acculturative Stress (ASISS)

The goal is to determine whether longer time spent in the host country correlates with meaningful changes in these psychological factors.

**Background of the Study**

The original research found that:

International students face higher mental health risks than the general population.

Two major predictors of depression are:

Social connectedness (sense of belonging)

Acculturative stress (stress of adapting to a new culture)

This project re-examines those relationships using SQL to compute aggregated metrics grouped by length of stay.

**Project Objective**

Using SQL (MySQL), generate a table with:

9 rows (one for each distinct length of stay)

5 columns:

Column	Meaning
stay	Years lived in host country
count_int	Number of international students in that stay period
average_phq	Mean depression score (PHQ-9), rounded to 2 decimals
average_scs	Mean social connectedness score (SCS), rounded to 2 decimals
average_as	Mean acculturative stress score (ASISS), rounded to 2 decimals

The results must include only international students, and be sorted by stay (descending).

Final result is stored in a DataFrame named df.

**Files Included**

- README.md               → Project documentation

- notebook.ipynb          → SQL analysis (DataCamp workbook)

- students.csv            → raw dataset

- SQL Query.sql           → SQL query used in the project

- df.csv                  → Exported aggregated results


**Dataset Description**

The students table includes the following fields:

Field	Description
inter_dom	Student type (international/domestic)
japanese_cate	Japanese language proficiency
english_cate	English language proficiency
academic	Academic level (undergraduate/graduate)
age	Student age
stay	Length of stay in years
todep	Depression score (PHQ-9 test)
tosc	Social connectedness score (SCS test)
toas	Acculturative stress score (ASISS test) 

**SQL Techniques Used**

Conditional filtering

Aggregation with AVG() and COUNT()

Rounding and aliasing

Grouping by categorical values

Sorting

Creating a final DataFrame named df

**Interpretation of the Output**

The resulting table allows us to analyze:

Whether longer residence reduces or increases depression scores

How length of stay affects social connectedness

Whether time in the host culture influences acculturative stress

Overall trends of emotional adjustment among international students

These patterns can guide universities in providing targeted mental health support.


