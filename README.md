# School District Analysis

## Overview of the School District Analysis

### Purpose

After completing the initial analysis of the School District, the school board notified the analytics team (Maria and her supervisor) that the students_complete.csv file showed evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have asked for help. 



### Methodology

The analysis was conducted using Jupyter notebook with pandas and numpy python language tools.

To determine the impact that the suspected fraud at Thomas High School (THS) has had on the overall performance of the school, a new dataframe was created in which the math and reading scores for THS ninth grade were replaced with null values,  NaNs, while keeping the rest of the data intact. 

Thomas High School 9th grade scores replaced with NaN
![GitHubLogo]()

To determine the impact of the changes a new school district analysis was run with the null values and compared to the original analysis.

Original School District Analyis File: [PyCitySchools.ipynb](insert here)

New School District Analysis File: [PyCitySchools_Challenge.ipynb](insert here)

A comparison was then done between the original school district analysis and the new school district analysis.


## Results

The results of the comparison between the original an new school district analyses follow.


### Impact on the Key School District Metrics

1. How is the district summary affected?


    Original District Summary
    
    ![GitHubLogo]()
    
    New District Summary

    ![GitHubLogo]()

2. How is the school summary affected?

    Original School Summary
    
      ![GitHubLogo]()

    New School Summary

     ![GitHubLogo]()


3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

     Changing Thomas High School's ninth graders' math and reading scores did not result in a change in Thomas High School's overall rnak in the school district. 
     They were ranked 3rd inthe district for overall scoring before and after the removal of the ninght grade scores.
     
     Original Top 5 Ranking:
        
      ![GitHubLogo]()

     New Top 5 Ranking:

      ![GitHubLogo]()

4. How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade

  The change in 9th grade math and reading scores for Thomas Hig School only resulted in a change only to the 9th grade math and reading scores overall.
  
  Original Math and Reading Scores by Grade
  
  ![GitHubLogo]()

  New math and reading Scores by Grade
  
  ![GitHubLogo]()

- Scores by School Spending

   Original scores by school spending
     
   ![GitHubLogo]()

   New Sores by school spending

    ![GitHubLogo]()

- Scores by School Size

   Original scores by school size

   ![GitHubLogo]()

   New scores by school size

   ![GitHubLogo]()

- Scores by School Type

    Original scores by school type

 ![GitHubLogo]()
 
    New   
 
  ![GitHubLogo]()
 
## Summary

Four major changes occurred in the analysis after Thomas High School ninth grade reading and math scores were replaced with NaNs.

1. 
2. 
3. 
4. 







