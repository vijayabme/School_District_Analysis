# School_District_Analysis

## Overview of the school district analysis:
### Purpose
The purpose of this analysis is to help a data scientist for a city school district in preparing the data from a variety of data sources, analyzing the data  and reporting about performance trends and patterns. These results and insights would help in making strategic decisions at the school and district level.    

### Software 
Python 3.7

## Results:
### District Summary:
The district summary indicates 
- There are a total of 15 schools in the district
- Total students across all the schools in the district is 39,170
- The total budget for the school district is $24,649,428
- Average math score is 78.9
- Average reading score is 81.9 
- Percentage of students passing math is 75%
- Percentage of students passing reading is 86%
- Overall passing percentage is 65%

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/district_summary_df.jpg)

### School Summary:
The summary for each school indicates 
- The pass percent is higher for charter schools compared to district schools.
- The district schools have a higher population than the charter schools

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/per_school_summary_df_after.jpg)

### Top 5 and bottom 5 performing schools
- The top 5 schools are all charter schools with less number of students.
- The bottom 5 schools are all district schools with more students.
- The budget for four of these charter schools for each student is slightly less than the dictrict schools.
- The average reading score is around 2% higher and math scores is on an average 7% higher for the charter schools  
- The percentage of students passing math is on an average 28% higher for charter schools
- The percentage of students passing reading is on an average 15% higher for charter schools
- The bottom performing district schools need improvement in math compared to the top performing charter schools
- 
![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/top5_bottom5_schools.jpg)
### Math and Reading scores in each grade level
Math scores are similar across the grades for each of the schools. But for some schools its in the 70% and for some schools its in the 80% range.

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/MathScores_by_grade.jpg)

Reading scores are similar across grades and they are all in the 80% range for all the schools.
Thomas High school 9th grade is not taken into account so its an nan for both math and reading scores

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/Reading_scores_bygrade.jpg)
### School performance based on the budget
The school performance and the spending ranges(Per Student) are inversely proportional.
The schools with less budget per student are showing higher performance in math and reading compared to the ones with higher budget.

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/Performance_budget.jpg)
### School performance based on the school size
Schools with small (<1000) and medium (1000-2000) size populations are doing better compared to schools with a large (2000-5000) population

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/Performance_SchoolSize.jpg)
### School performance based on the school type
Charter Schools are performing better than district schools.

![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/Performance_SchoolType.jpg)

## Summary:
For Thomas High School replacing the 9th grade reading and math scores to nan, reduced the percentage of students that passed reading, math and both reading and math 
- % passing reading became 67%
- % passing math became 70%
- % overall passing became 65%
![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/ThomasHighSchool_summary_beforeremoving_nancount.jpg)
Once the subjects with Nans were removed from the subject count and the percentage was calculated, the percentages are similar to what we had before adding the NaNs. 
There are only 461 students in 9th grade which is a small number compared to the 10th, 11th and 12th combined. So removing them didn't affect the overall percentage by much
![image](https://github.com/vijayabme/School_District_Analysis/blob/main/Resources/ThomasHighSchool_summary_after_removingnancount.jpg)

- School performance didnt get better with school spending budget for each student. The charter schools that had a lower budget for each student had higher performance
- School size matters a lot when it comes to student performance. The district schools with higher populations had lower performance compared to charter schools with lower population.
- Overall charter schools had better performance than district schools.
- The math scores are the ones that are dropping more in district schools compared to charter schools. The reading scores are similar across both kind of schools.  The charter schools with less kids might be giving a better one on one attention to students which might be contributing towards the students success.



