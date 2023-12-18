# pandas_challenge - Module 4

# Overview
In this challenge, Pandas DataFrames were leveraged to analyze school and standardized test data.

# Technologies
* Python
* Pandas
  
# District Summary
After obtaining the starter files, key district metrics were calculated and stored in a DataFrame named "district_summary":

* Total number of unique schools: 15
* Total students: 39,170
* Total budget: $24,649,428
* Average math score: 78.99%
* Average reading score: 81.88%
* % Passing Math: 74.98%
* % Passing Reading: 85.81%
* % Overall Passing: 65.17%
<img width="1013" alt="Screenshot 2023-12-18 at 1 54 07 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/6a772719-d688-49d7-befd-dac85d8989d1">

# School Summary
Upon completing district calculations, a "per_school_summary" DataFrame was created, summarizing key metrics for each school:

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
Top and bottom performing schools were identified based on "% Overall Passing" and saved as "top_schools" and "bottom_schools" DataFrames, respectively.
<img width="1319" alt="Screenshot 2023-12-18 at 1 55 11 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/201280ec-7bd8-40b7-975d-3254095f5797">

# Math & Reading Scores by Grade
Average math and reading scores were calculated for each grade (9th, 10th, 11th, 12th) using the groupby function.
<img width="730" alt="Screenshot 2023-12-18 at 1 59 34 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/e5c8d117-3011-4e9c-bd65-463433693f41">
<img width="756" alt="Screenshot 2023-12-18 at 1 59 46 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/5bbd3f56-d13f-4a07-9191-03cd92a0e4c9">

# Scores by School Spending
A table breaking down school performance based on average spending per student was created using predefined bins and pd.cut. The results were stored in a "spending_summary" DataFrame.
<img width="889" alt="Screenshot 2023-12-18 at 2 03 09 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/f175b101-bcaa-4da9-8a12-1dadafbec150">

# Scores by School Size
School performance was categorized based on school size (small, medium, or large) using the "per_school_summary" DataFrame and stored in a "size_summary" DataFrame.
<img width="963" alt="Screenshot 2023-12-18 at 2 08 40 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/c1817240-88a2-41bf-b5ec-fb601acc8058">


# Scores by School Type
Average test scores for reading and math were calculated by school type using the "per_school_summary" DataFrame, and the results were saved in a "type_summary" DataFrame.
<img width="870" alt="Screenshot 2023-12-18 at 2 07 42 PM" src="https://github.com/samkimmmm/pandas_challenge/assets/135805393/de74a316-d4de-42f0-9eb7-1d73a58a6d1f">

# Analysis Report
Findings from the analysis include:
1. Schools with higher budgets did not necessarily yeild better test results. Schools with spending between $645-675 per student underperformed compared to those with smaller budgets ($585 per student).
2. Smaller and medium-sized schools outperformed large-sized schools significantly in math performance (89-91% passing vs. 67%).
3. Charter schools consistently outperformed public district schools across all metrics, prompting further analysis to determine whether this effect stems from school practices or smaller student populations.
