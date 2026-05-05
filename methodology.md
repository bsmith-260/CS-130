# Methodology of Graduate Data 

## Data Sources
-I downloaded the dataset graduates.csv from the CORGIS Dataset Project.

-The Website Source: https://corgis-edu.github.io/corgis/csv/graduates/

-The dataset contains information about graduates by year and major, including demographic counts, degree totals, salary statistics, employment status, employer type, and work activity.

-I used graduates.csv as the primary data source for my analysis.

## Data Preparation/Cleaning
-I started by checking for any missing values across all of the columns to identify whether any years, majors, salary fields, or employment fields were incomplete, or missing.

-I verified that all of the columns in the data set such as Salaries.Mean, Salaries.Quantity, etc., were stored as numeric data values and could be used in my calculations.

-I imported the CSV into a pandas DataFrame and reviewed it using .head(), .shape, .columns, and .info() to understand the structure of the dataset.

-I examined the Education.Major column for duplicate or inconsistent major names and standardized them if needed so that the same major was not counted under slightly different names.

-I checked whether category totals were logical and consistent. For example, I compared Demographics.Gender.Females plus Demographics.Gender.Males to Demographics.Total, and I compared Employment.Status.Employed, Employment.Status.Unemployed, and Employment.Status.Not in Labor Force to overall totals to look for any errors.

## Assumptions
-I assumed that salary values from different years could be compared in a meaningful way, even though the dataset description did not clearly state whether the salaries were adjusted for inflation.

-I assumed that broad categories such as Minorities were defined consistently across all years in the dataset.

-I assumed that the reported salary statistics were based on reliable self-reported or collected salary information, even though the dataset does not fully explain the reporting process.

-I assumed that when comparing majors, differences in salary or employment reflected real differences in outcomes, even though the dataset does not include other factors like region, age, or years of experience.

## Limitations
-One of the limitations of the graduates data set that I observed was the lack of information for some of the different data points. For a large portion of the available college graduate degrees, there is no data before the year 2008, which is the majority of the time frame, as the complete data set is from the year 1993 to 2015.

-With the dataset being set from 1993 to 2015, the data does not reflect the up to date information on data points such as salary, employment and education trends.

-With the data being primarily organized by major and year, it does not take into consideration each individuals personal graduate experience within that degree, or any circumstances they may have faced that have affected their abilities to work a job within the specific degree in which they graduated with.

-The dataset includes a lowest salary of 0.0 in some cases, which may reflect unusual reporting, missing context, unpaid work, or another special case. Without more documentation, I cannot fully interpret what a salary of 0 means.