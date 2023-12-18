# pandas_challenge
Module 4 Challenge

In this challenge, I created and manipulated Pandas Dataframes to analyze school and standardized test data.

Language(s) used: Python
Database used: Pandas

# District Summary
After downloading the starter files, I had calculated key metrics of the district, including the following, and saved the results into a DataFrame:
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
Once the district calculations were complete, I then calculated key metrics for each school and created a DataFrame with the following columns:
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

# Highest and Lowest Performing Schools (by % Overall Passing)
I sorted the schools by "% Overall Passing" in descending order, displayed the first 5 rows, then saved the results as a new DataFrame called "top_schools". I repeated this process in ascending order for the lowest performing schools and dsaved the results as a new DataFrame called "bottom_schools".

# Math & Reading Scores by Grade
I performed 
