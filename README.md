# School District Analysis

## Overview

### Background

The purpose of the original School District Analysis, corresponding to the PyCitySchools.ipynb script found in this repository, was to analyze relevant metrics associated with various students that attend several schools within a certain school district. 

### Purpose

The purpose of the Challenge was to clean the information used in the original School District Analysis, so as to account for incorrect information concerning Thomas High School's ninth grade students scores, then, perform a new analysis, and finally, contrast the results of the new analysis with the original one.

### Cleaning the data

The incorrect data associated with Thomas High School's ninth grade math and reading scores was replaced with "Nan" using the "loc" method available for pandas dataframes using the following code:

```
student_data_df.loc[(student_data_df["school_name"]=="Thomas High School")&(student_data_df["grade"]=="9th"), "reading_score"]=np.nan

student_data_df.loc[(student_data_df["school_name"]=="Thomas High School")&(student_data_df["grade"]=="9th"), "math_score"]=np.nan

```

## Results

The pertinent metrics associated with most of the results are Total Students (TS), Per Student Budget (SB), Average Math Scores (AMS), Average Reading Scores (ARS), % Passing Math (PM), % Passing Reading (PR), and % Overral Passing (OP). 

Given that only Thomas High School's ninth grade scores were cleaned to adjust incorrect information, and these are involved only in the calculation of AMS, ARS, PM, PR, and OP, both TS and SB will not be addressed in the remaining of this section, as results for these two metrics in the new analysis were identical to those made previously in the original analysis. (**Note**: that this implies that for all results related to AMS, ARS, PM, PR, and OP, the cleaning of the data did produce an alteration on the metric. However, not in all cases was the alteration significant enough as to create a difference in the final metric because the final metric was rounded for presentation purposes.) Any omission of the aforementioned 5 metrics in the following subsections is to be interpreted as implying that the metric did not sufffer significant changes in the new analysis.

### District Summary

* Given that the District Summary represents aggregation up to the district level, metrics AMS, PM, PR, and OP were all negatively affected by the cleaning of the data.

### School Summary

* Given that the School Summary represents aggregation up to the school level, only Thomas High School's results were affected by the cleaning of the data. Specifically, PM, PR, and OP, saw a decrease in the new analysis with respect to the original.

### Thomas High School's Performance Relative to Other Schools

* Thomas High School's performance, as measured by AMS, PM, PR, and OP, was negatively affected, relative to other schools, by the removal of incorrect scores information for ninth graders associated with that school.

### Math and Reading Scores by Grade

* Given that the results are aggregated at the school level and grouped by grade, the only change in the new analysis with respect to the original one was that in the new analysis Thomas High School's ninth grade results are not available, which is consistent with the cleaning of the data performed to invalidate incorrect information.

### Scores by School Spending

* The aggregation for this result was performed with bins, and given Thomas High School's school spending per student of $638, bin "$630-$644" metric for PM was negatively affected by the cleaning of the data.

### Scores by School Size

* The aggregation for this result was performed with bins, and given Thomas High School's total student count of 1636 (which implies a classification of size as "Medium"), the "Medium" bin was negatively affected by the cleaning of the data, but the alteration was not significant enough to imply a relevant diference in the final metric. (see **Note** above)

### Scores by School Type

* The aggregation for this result was performed on school type, and given that Thomas High School is a "Charter", that category's results were negatively affected by the cleaning of the data, but the alteration was not significant enough to imply a relevant diference in the final metric. (see **Note** above)

## Summary

### Four changes in the updated School District Analysis

1) District Summary's results in the original analysis for the metrics AMS, PM, PR, and OP, decreased by 0.1, 0.2, 0.1, and 0.3, respectively, in the new analysis.
2) In Schools Summary, Thomas High School's results in the original analysis for the metrics PM, PR, and OP, decreased by 0.1, 0.3, and 0.4, respectively, in the new analysis.
3) In Scores by School Spending Size, bin "$630-$644"'s results for the metric PM decreased by 1.0 when rounded up to the ones.
4) On the rest of the results, differences in metrics between the original and new analysis were not considerable enough to create alterations in the final metrics. (see **Note** above)


