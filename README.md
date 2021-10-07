# School District Analysis

## Overview

### Background

The purpose of the original School District Analysis, corresponding to the PyCitySchools.ipynb script found in this repository, was to analyze relevant metrics associated with various students that attend several schools within a certain school district. 

### Purpose

The purpose of the Challenge was to clean the information used in the original School District Analysis, so as to account for incorrect information concerning Thomas High School's ninth grade students scores, then, perform a new analysis, and finally, contrast the results of the new analysis with the original one.

## Results

Given that only Thomas High School's ninth grade scores were cleaned to adjust incorrect information, out of the 7 metrics associated with each school, Total Students and Spending per Student were not affected at any level by the alteration of the data. In consequence, in what remains of this section, these two metrics will not be addressed.

### District Summary

* Given that the District Summary represents aggregation up to the district level, the original results were affected by the cleaning of the data.

### School Summary

* Given that the School Summary represents aggregation up to the school level, only Thomas High School's results were affected by the cleaning of the data.

### Thomas High School's Performance Relative to Other Schools

* Thomas High School's performance, as measured by Average Math Scores (AMS), Average Reading Scores (ARS), % Passing Math (PM), % Passing Reading (PR), and % Overral Passing (OP), were negatively affected by the cleaning of the data in four out of five metrics (that is, all but ARS).

### Math and Reading Scores by Grade

* Given that the results are aggregated at the school level and grouped by grade, the only change in the new analysis with respect to the original one was that in the new analysis Thomas High School's ninth grade results are not available, which is consistent with the cleaning of the data performed to invalidate incorrect information.

### Scores by School Spending

* The aggregation for this result was performed with bins, and given Thomas High School's school spending per student of $638, the only bin affected by the cleaning of the data was "$630-$644".

### Scores by School Size

* The aggregation for this result was performed with bins, and given Thomas High School's total student count of 1636 (which implies a classification of size as "Medium"), the only bin affected by the cleaning of the data was the "Medium" bin.

### Scores by School Type

* The aggregation for this result was performed on school type, and given that Thomas High School is a "Charter", only that category's results were affected by the cleaning of the data.

## Summary

### Four changes in the updated School District Analysis

1) District Summary's results in the original analysis for the metrics AMS, PM, PR, and OP, decreased by 0.1, 0.2, 0.1, and 0.3, respectively, in the new analysis.
2) In Schools Summary, Thomas High School's results in the original analysis for the metrics PM, PR, and OP, decreased by 0.1, 0.3, and 0.4, respectively, in the new analysis.
3) In Scores by School Spending Size, bin "$630-$644"'s results for the metric PM decreased by 1.0 when rounded up to the ones.
4) On the rest of the results, differences in metrics between the original and new analysis were not considerable enough to create alterations after rounding the numbers.


