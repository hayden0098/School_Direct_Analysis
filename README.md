# School_Direct_Analysis
using Anaconda Jupeter Notebook

## Overview of School Direct Analysis:
Using Python and Pandas library to analyse the dataset of student funding and student's standardized test score assists school board make decision of upcoming school year's school budgets and priorities. After cleaning the dataset by checking missing values, fixing the pre/suffix name, and not counting the data of 9th grade student at Thomas High school since the evidence of academic dishonesty, we generate the summary of district that provides all schools data, an overview summary of key metrics for each school, Top 5 Bottom 5 overall passing rate performing school, average student's math and reading score in each grade level at each school as well as the shcool performance based on budget perstudent, school size and type of school. 

## School Direct Analysis Resaults:

- ###### How is the district summary affected?
Before:

![district_summary_df_before](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/district_summary_df_before.png)

After:

![district_summary_df_after](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/district_summary_df_after.png)

As the affected of Thomas High school academic dishonesty the average of Math, reading score and their passing percentage were droped down by 5~10 %, but the overall passing percentage rate were raised a bit up since we are not counting some THS student and reade their score as None, so their score are not count while we calculating the average score, and passing percentage rate.

- ###### How is the school summary affected?
Before:

![per_school_summary_before](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/per_school_summary_before.png)

After:

![per_school_summary_after](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/per_school_summary_after.png)

As the affected of Thomas High school academic dishonesty, it wont affected other shcool data, the only affected is THS row in the shcool summary. compare to the table before academic dishonesty, we see that the percentage of passing in math, reading and overall are having droped a bit. Also the average of math and reading change are relativly small.

- ###### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Before:

![top_5_performaing_before](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/top_5_performaing_before.png)

After:

![top_5_performaing_after](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/top_5_performaing_after.png)

Replacting the 9th graders' math and reading scores with None, this must affect Thomas High School's sum and the averages of the scores becuase those number of Nones will not be considered in the calculation. Compare to the other schools, THS have less student that participate the standardized test which gives THS having less population number. In the performance of top 5 schools, THR still have 2nd top place compare. 

- ###### How does replacing the ninth-grade scores affect the following:
	- ###### Math and reading scores by grade
		Replacting the 9th graders' math and reading scores with None, In the table of scores by grade the Math and Reading scores for grade 9th will become None, and for the rest of grade 10th, 11th,12th doesn't get any affect.
    Reading Score:
    
		![reading_scores_by_grade](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/reading_scores_by_grade.png)
    
    Math Score:
    
    ![math_scores_by_grade](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/math_scores_by_grade.png)
	
	- ###### Scores by school spending
		Replacting the 9th graders' math and reading scores with None, In the table of scores by school spending don't have any affect, since the numbers of students for each school are remain the same, the student information in the row which score have replace with None still counted.  the None score just affected the calculation of sum and average.

		![spending_summary_df](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/spending_summary_df.png)
    
	- ###### Scores by school size
		Replacting the 9th graders' math and reading scores with None, In the table of scores by school size don't have any affect, since the numbers of students for each school are remain the same, the student information in the row which score have replace with None still counted.  the None score just affected the calculation of sum and average.

		![size_summary_df](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/size_summary_df.png)

	- ###### Scores by school type
		Replacting the 9th graders' math and reading scores with None, In the table of scores by school type don't have any affect, since the numbers of students for each school are remain the same, the student information in the row which score have replace with None still counted.  the None score just affected the calculation of sum and average.

		![type_summary_df](https://github.com/hayden0098/School_Direct_Analysis/blob/main/Resources/Screenshot/type_summary_df.png)

## Summary:
As result of replaced the reading and math scores with None, the changes in the updated school district analysis:

	1. In District Summary, The Average score of reading and math decreased, The percentage of Passing rate decreased also .

	2. In School Summary, Only in Thomas High school the percentage of passing in math, reading and overall decreased

	3. Every Grade 9th student's math and reading averagescore at Thomas High School and its average score becomes None, also the percentage of passomg rate for math, reading, and both will change
	
	4.  Since the student data other than math, reading score are not removed from the dataset, basically the total student remain unchanged. Therefore the deducted student count will only consider when calculating the average score and passing rate.

