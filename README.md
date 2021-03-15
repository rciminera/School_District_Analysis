# School District Analysis
by Bob Ciminera

## Overview of the School District Analysis

### Purpose

Maria is a data scientist for a city school district responsible for preparing standardized test date for analysis, reporting, and presentation to provide insights about performance trends and patterns. These insights are used to inform discussions and strategic decisions at the school and district level.

For this analysis, Maria was provided school funding and other data as well as student results on standardized math and reading tests. With my assistance, her task was to aggregate this data to showcase trends in school performance.

This will assist the school board and superintendent in making decisions regarding school budgets and priorities.

After completing the initial analysis of the School District, the school board notified the analytics team that the students_complete.csv file showed evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. 

Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have asked for help. 


### Methodology

The analysis was conducted using Jupyter notebook with pandas and numpy python language tools.

In the original analysis the data was munged to preifxes and suffixes such as "Dr." and "Jr."  

In the second version of the analyis the data was again munged to determine the impact that the suspected fraud at Thomas High School (THS) has had on the overall performance of the district and school.

This was accomplished by creating a new dataframe in which the math and reading scores for THS ninth grade were replaced with null values,  NaNs, while keeping the rest of the data intact. 

To determine the impact of these changes a new school district analysis was run and compared to the original analysis to see what impact these changes has on the analysis.

The school district analysis code can be found here: [PyCitySchools_Challenge.ipynb](PyCitySchools_Challenge.ipynb)

Snippet of code used to replace Thomas High School 9th grade scores with NaN:

![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/Replace%20scores%20with%20nan.png)


## Results of the School District Analysis

Following are the results of the comparison between the original analyis and the new school district analysis after the THS ninth grade math and reading scores were removed.

### 1. Impact on the Key School District Metrics

The new district summary changed slightly from the original with a 30bps drop in students % Overall Passing.  This came with with a 20bps drop in % Passing Math and a 10bps drop in % Passing Reading. 

District Summary New vs Original    
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/DistrictCompare.png)
   
### 2. Affect on School Summary

In the new analysis, removing grades from 461 THS ninth graders naturally had no impact on other schools performance. The impact on THS % Overall Passing was 30 bps with % Passing Math showing virtually no drop and % Passing Reading down by 20bps. 

New School Summary:
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewSchoolSummary.png)

Original School Summary:    
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/OriginalSchoolSummary.png)

Thomas High School Comparison:
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/ThomasHS.png)

### 3. Affect on Thomas High School’s Relative Performance 

Thomas High School's rank of 2nd among the 15 high schools did not change.

New Top 5 Ranking:
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/OriginalTopandBottomSchools.png)

Original Top 5 Ranking:        
![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewTopandBottomSchools.png)

### 4. How does Replacing the Ninth-Grade Scores Affect the Following?

- Math and Reading scores by Grade

  The change in 9th grade math and reading scores for Thomas High School only resulted in a change only to the 9th grade math and reading scores overall. 
  
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewMathScoresbyGrade.png)
  
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewReadingScoresbyGrade.png)
  
- Scores by School Spending

  There were no changes to scores by school spending. 

  Original scores by school spending:     
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/OriginalSpendingSummary.png)

  New Scores by school spending:
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewSpendingSummary.png)

- Scores by School Size

  There were no changes to scores by school size.

  Original scores by school size:
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/OriginalSizeSummary.png)

  New Scores by School Size:
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewSizeSummary.png)

- Scores by School Type

  There were no changes to scores by school type

  New Scores by School Type:
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/NewTypeSummary.png)
 
  Original Scores by School Type:
  ![GitHubLogo](https://github.com/rciminera/School_District_Analysis/blob/main/Screen_Shots/OriginalTypeAnalysis.png)
 
## Summary

In reviewing the analysis after Thomas High School ninth grade reading and math scores were replaced with NaNs,
the most significant finding is that the difference in the analysis without the 9th grade scores is unremarkable.

The four major findings are as follows:

1. District % Overall Passing was down after the changes but only by (30bps)
2. Thomas High School's ranking at 2nd in the district did not change.
3. There were no changes to Scores by School Size, Type, or Spending
4. 



