# School_District_Analysis
## Overview of the School District Analysis
### Background
The school board has uncovered evidence of academic dishonesty.  The full extent is unknown.  Alteration of reading and math grades for Thomas High School ninth graders are at issue.  Maria has asked for a full audit after replacement of the math and reading scores for Thomas High School ninth graders with NaNs (referred to as Data Cleanup below), while making no other changes to the data. Once the revision has been made, Maria has requested a repeat run of the school district analysis (with the suspect grades not considered) and a report detailing how the data changes affected the overall analysis.

### Deliverables requested include:
* District summary DataFrame 
* School summary DataFrame 
* Tables presenting the following metrics:
    * Top 5 performing schools, based on the overall passing rate 
    * Bottom 5 performing schools, based on the overall passing rate 
    * Average math score for each grade level from each school 
    * Average reading score for each grade level from each school 
    * School performance by school spending per student 
    * School performance by school size 
    * School performance by school type 

### Results: 

#### How is the District Summary affected?
#### District Summary (excluding 9th grader scores from Thomson High School)
Analysis before and after the math and reading scores of Thomas High School 9th graders were changed to Nans (Data Cleanup) will cover the Distric Summary, School Summary, School average scores and School performance by spending, size and type.

#
#### Before data cleanup: 
* average math score, average reading score, % passing math, % passing reading, % passing math and reading
* 79.0, 81.9, 75, 86, 65
#### After data cleanup
* average math score, average reading score, % passing math, % passing reading, % passing math and reading
* 78.9, 81.9, 74, 85, 64
#
#### Before Data Cleanup Summary Table
![District Summary](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/districtsummarybefore.PNG)
#### After Data Cleanup Summary Table
![District Summary](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/districtsummary.PNG)
#
#### Findings
* Small changes in the overall average math and reading scores
* Small changes in the % of students passing math
* Small changes in % of students passing reading 
* Small changes in % of both passing math and reading
#
#### How is the School Summary affected?
* Before data cleanup, Thomas School overall passing rate was 2nd in the district, with an overall passing rate of 91%
* After data cleanup, Thomas School overall passing rate was  8th in the district, with an overall passing rate of 65%
* After data cleanup, Thomas School overall performance ranking sank from 2nd to 13th (out of 15)
* The data cleanup revealed much worse results both in school ranking and overall passing rate for Thomas High School
#### School Summary
![School Summary](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/school_summary.PNG) 
#
### Top 5 performing schools (based on passing rate)
![Top 5 performing schools](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/topfive.PNG)
### Bottom 5 performing schools (based on passing rate)
![Bottom 5 performing schools](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/bottom5.PNG)
#
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
#
## Thomas School math and reading scores for 9th graders were replaced with NaN (not a number)
### School Math scores by grade
![School Math Score Averages](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/averagemath.PNG)
### School Reading Scores by grade
![School Reading Score Averages](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/averagereading.PNG)
## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?



How does replacing the ninth-grade scores affect the following:
## Math and reading scores by grade
## Scores by school spending
## Scores by school size
## Scores by school type
## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.