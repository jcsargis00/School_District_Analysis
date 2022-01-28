# School_District_Analysis
## Overview of the School District Analysis
### Background and Purpose
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
#### Data Preparation
* Correct student names to remove prefixes and suffixes
* Replace Thomas High School 9th grade reading and math scores with NaN
* Use cleaned data to rerun analysis and report any changes to the results 

### Results 
Analysis before and after the math and reading scores of Thomas High School 9th graders were changed to Nans (Data Cleanup).  This report will look at changes to the District Summary, School Summary, School average scores and School performance by spending, size and type.
#### How is the District Summary affected?
#### District Summary DataFrame
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
* District averages went down slightly
#
#### How is the School Summary affected?
#### School Summary DataFrame
* Before data cleanup, Thomas School overall passing rate was 2nd in the district, with an overall passing rate of 91%
* After data cleanup, Thomas School overall passing rate was  8th in the district, with an overall passing rate of 65%
* After data cleanup, Thomas School overall performance ranking sank from 2nd to 13th (out of 15)
* The data cleanup revealed much worse results both in school ranking and overall passing rate for Thomas High School
#### School Summary Table
The School Summary Table after data cleanup shows Thomas High School ranked 13th out of 15 schools in the district.
![School Summary](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/school_summary.PNG) 
#
#### Top 5 performing schools (based on passing rate) 
Before data cleaning, Thomas High School ranked 2nd, a top 5 performing school.  
After, Thomas High School ranked as a bottom 5 performing school
![Top 5 performing schools](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/topfive.PNG)
#### Bottom 5 performing schools (based on passing rate) 
![Bottom 5 performing schools](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/bottom5.PNG)
#
#### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
#### Thomas High School math and reading scores for 9th graders before data cleaning
#
![Reading and Math Scores before dc](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/schooloverallbefore.PNG)
#### Thomas School math and reading scores for 9th graders after data cleaning
Setting up a boolean test and using loc and len on the student_data.df to find the number of 9th graders at Thomas High School. 461 students were in 9th grade at Thomas High School. Before data cleanup there were 1635 students, after there were 1174 (after removing the 461 9th graders scores).
#
![9th graders](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/ninthgraders.PNG)
####  Their reading and math scores were set to NaN and the overall passing report was rerun with the following result.
![Reading and Math Scores after dc](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/schooloverallpassingafter.PNG)
#
How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
#### Average School Math scores by grade for each school
#
![School Math Score Averages](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/averagemath.PNG)
#### Average School Reading Scores by grade for each school
#
![School Reading Score Averages](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/averagereading.PNG)
#### Scores by school spending
Thomas High School is in spending bin ranging from $630-644
#
* Before: Passing % in Math, Reading, Overall= 73, 84, 63 
* After:  Passing % in Math, Reading, Overall= 67, 77, 56  a significant dropoff in performance
#### Summary Table of School Spending per student
![spending per student](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/spendingperstudentafter.PNG)

#### Performance scores by school size 
![school size](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/spendingbyschoolsize.PNG)

#### Performance scores by school type
![school type](https://github.com/jcsargis00/School_District_Analysis/blob/main/Resources/spendingbyschooltype.PNG)

### Summary
#### Changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
* Removing 9th grade student scores from Thomas High School affected the school district in the following ways:

Average math scores dropped slightly (<1%)
Average reading scores were not affected
Percentage of students passing math dropped slightly (-1%)
Percentage of students passing reading dropped slightle (-1%)
The overall passing rate dropped (-1%)
Only scores for Thomas High School were affected:

Perentage of students passing math dropped from 93.2% to 66.9%
Percentage of students passing reading dropped from 97.3% to 69.7%
Overall passing percentage dropped from 90.9% to 65.1%
Thomas High School affected school rankings in the following ways:

Thomas High school dropped out of the top 5 high schools in the district
Wright High School moved into the top 5 high schools in the district
Bottom 5 high schools was unaffected
Removing 9th grade student scores from Thomas High School affected other reports:

Math and reading scores by grade remained the same for all other schools
Thomas High School had no data to report for 9th grade math and reading scores
Scores by school spending chaged at the $601-650 range:
Percentage passing math dropped from 73% to 67%
Percentage passing reading dropped from 84% to 77%
Overall passing percentage dropped from 63% to 56%
Scores by school size changed for medium-sized schools (1000-2000):
Percentage passing math dropped from 94% to 85%
Percentage passing reading dropped from 97% to 91%
Overall passing percentage dropped from 91% to 85%
Scores by schools type were affected in the following ways:
Percentage passing math dropped from 94% to 90%
Percentage passing reading dropped from 97% to 93%
Overall passing percentage dropped from 90% to 87%
* 
* 
* 