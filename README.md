# PyCitySchools_Challenge

# Overview of the school district analysis
We have data from the school district with students' names, their math scores, reading scores, which schools they go to and, which district those schools are in, and etc. 
It's much of information and we are tring to clean up some of the areas in the data and figure out what the data is telling us; 
how different the math and reading scores are by school, how much money the schools are spending, how that is related to the students' scores and, 
which grade is doing better for each school. 

# Results

### How is the district summary affected?

![district_summary_original](./Resources/district_summary_df_original.png)
As you can see the screenshot above which is the original district summary data frame, Passing Math Percentage was 75.0% and Passing Reading Percentage was 85.8%, 
and the Overall Passing Percentage was 65.2%. 

![district_summary_df_changed](./Resources/district_summary_df_changed.png)
What we have changed here was the student count: The original district summary data frame was with the total number of students, but here we subtracted the number of students 
that are in ninth grade at Thomas High School from the total student count to get the new total student count. 
So, the new total student (without 9th graders' scores) count was reflected into our passing math, reading, and overall percentages. 

% of Passing Math: 75.0% -> 74.8%  //
% of Passing Reading: 85.8% -> 85.7%  //
% of Passing Overall: 65.2% -> 64.9%

### How is the school summary affected?

![per_school_summary_df_original](./Resources/per_school_summary_df_original.png)
As you can see the screenshot above, the original per school summary data frame, passing math percentage was 66.9%, passing reading percentage was 69.7%, and
the overall passing percentage was 65.1%. 

![per_school_summary_df_changed](./Resources/per_school_summary_df_changed.png)
We changed the graders to only 10th to 12th graders at Thomas High School. 
So, the new grader group was reflected into our passing math, reading, and overall percentages. 
% of Passing Math: 66.9% -> 93.2%  //
% of Passing Reading: 69.7% -> 97.0%  //
% of Passing Overall: 65.1% -> 90.6%

As you can see, the percentages all went up by a lot for all categories which tells us that the from 10th to 12th graders at Thomas High School did very well
on Math, Reading, and overall! 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
The percentages all went down, but not by much. The district summary data numbers without 9th graders affected our original data by going down, 
which shows that the passing students from the 9th graders at Thomas high school actually was helping the other schools' passing percentages. 



### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade


#### Scores by school spending


#### Scores by school size


#### Scores by school type

