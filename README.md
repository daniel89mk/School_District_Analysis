# PyCitySchools_Challenge

# Overview of the school district analysis
We have data from the school district with students' names, their math scores, reading scores, which schools they go to and, which district those schools are in, and etc. 
It's much of information and we are tring to clean up some of the areas in the data and figure out what the data is telling us; 
how different the math and reading scores are by school, how much money the schools are spending, how that is related to the students' scores and, 
which grade is doing better for each school. 

# Results

### How is the district summary affected?

![district_summary_original](./Resources/district_summary_df_original.png)
The original data was after we replaced the 9th grade reading and math scores at Thomas High School with NaN.
This is the result from the original district summary data, and the passing Math percentage was 75.0% and Passing Reading Percentage was 85.8%, 
and the Overall Passing Percentage was 65.2%. 

![district_summary_df_changed](./Resources/district_summary_df_changed.png)
What we have changed here was the student count: The number of students that are in ninth grade at Thomas High School who had no grades was 461. And here we subtracted 
461 from the total student count to get the new total student count, which results in having 38709, new student count. 
So, the new total student (without 9th graders' scores) count was reflected into our passing math, reading, and overall percentages. 
The percentages all went down, but not by much.

% of Passing Math: 75.0% -> 74.8%  //
% of Passing Reading: 85.8% -> 85.7%  //
% of Passing Overall: 65.2% -> 64.9%

It shows that cleaning the 9th graders that had no grades did not affect the district summary much, but by removing them, the percentages went down.

### How is the school summary affected?

![per_school_summary_df_original](./Resources/per_school_summary_df_original.png)
As you can see the screenshot above, the original per school summary data frame, passing math percentage was 66.9%, passing reading percentage was 69.7%, and
the overall passing percentage was 65.1%. (The original school summary had all graders including 9th graders that had no grades.)

![per_school_summary_df_changed](./Resources/per_school_summary_df_changed.png)
We replaced the Thomas High School graders' numbers to only 10th to 12th graders at Thomas High School. 
So, the new grader group which became our numerator in the percentage calculation and our passing math, reading, and overall percentages went up! 

% of Passing Math: 66.9% -> 93.2%  //
% of Passing Reading: 69.7% -> 97.0%  //
% of Passing Overall: 65.1% -> 90.6%

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Replacing the ninth graders' math and reading scores definitely affected Thomas High School's performance by a lot.
Their overall passing percentage was 65.1% which was really low and it went up to 90.6%, then they got into the top 5 schools. 

### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade
![math_scores_by_grade](./Resources/math_scores_by_grade.png)
![reading_scores_by_grade](./Resources/reading_scores_by_grade.png)

By replacing 9th-grade scores to 10th-12th-grade scores, the math and reading scores by grade went down. 

#### Scores by school spending
![scores_by_school_spending](./scores_by_school_spending.png)

#### Scores by school size
![scores_by_school_size](./Resources/scores_by_school_size.png)

#### Scores by school type
![scores_by_school_type](./Resources/scores_by_school_type.png)
