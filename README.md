# pandas_challenge
Module 4 Challenge

In this challenge, I created and manipulated Pandas Dataframes to analyze school and standardized test data.

Language(s) used: Python
Database used: Pandas

# District Summary
After downloading the starter files, I had calculated key metrics of the district, including the following, and saved the results into a DataFrame titled "district_summary":
* Total number of unique schools: 15
* Total students: 39170
* Total budget: $24,649,428
* Average math score: 78.99%
* Average reading score: 81.88%
* Percentage of students who passed math: 74.98%
* Percentage of students who passed reading: 85.81%
* Percentage of students who passed both math AND reading: 65.17%
<img width="1013" alt="Screenshot 2023-12-18 at 1 54 07 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/6a772719-d688-49d7-befd-dac85d8989d1">

# School Summary
Once the district calculations were complete, I then calculated key metrics using groupby and value_counts() for each school and created a DataFrame titled "per_school_summary" with the following columns:
* School name (Index)
* School Type
* Total Students
* Total School Budget
* Per Student Budget
* Average Math Score
* Average Reading Score
* % Passing Math
* % Passing Reading
* % Overall Passing
<img width="1300" alt="Screenshot 2023-12-18 at 1 54 41 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/c845512f-a7f4-444f-a4d4-60401849716b">

# Highest and Lowest Performing Schools (by % Overall Passing)
I sorted the schools by "% Overall Passing" in descending order, displayed the first 5 rows, then saved the results as a new DataFrame called "top_schools". I repeated this process in ascending order for the lowest performing schools and dsaved the results as a new DataFrame called "bottom_schools".
<img width="1319" alt="Screenshot 2023-12-18 at 1 55 11 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/201280ec-7bd8-40b7-975d-3254095f5797">

# Math & Reading Scores by Grade
Using the groupby function, I calculated the average math and reading scores for each individual grade (9, 10, 11, 12) and created a dataframe for math and reading.
<img width="730" alt="Screenshot 2023-12-18 at 1 59 34 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/e5c8d117-3011-4e9c-bd65-463433693f41">
<img width="756" alt="Screenshot 2023-12-18 at 1 59 46 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/5bbd3f56-d13f-4a07-9191-03cd92a0e4c9">

# Scores by School Spending
In this section, I created a table that breaks down school performance based on average spending ranges per student. Using the provided bins, code, and pd.cut, I calculated the mean scores per spending range and created a DataFrame called "spending_summary". This DataFrame includes the following metrics:
* Average math score
* Average reading score
* % Passing Math
* % Passing Reading
* % Overall Passing
<img width="889" alt="Screenshot 2023-12-18 at 2 03 09 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/f175b101-bcaa-4da9-8a12-1dadafbec150">

# Scores by School Size
In this section, using the provided code and pd.cut on the "Total Students" column in the "per_school_summary" DataFrame, I created a new DataFrame titled "size_summary" that breaks down school performance based on school size (small, medium, or large).
<img width="963" alt="Screenshot 2023-12-18 at 2 08 40 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/c1817240-88a2-41bf-b5ec-fb601acc8058">


# Scores by School Type
Using the "per_school_summary" DataFrame, I calculated the average test scores of reading and math, grouped by school type, then saved the results into a new DataFrame titled "type_summary".
<img width="870" alt="Screenshot 2023-12-18 at 2 07 42 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/de74a316-d4de-42f0-9eb7-1d73a58a6d1f">
