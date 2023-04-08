## pandas-challenge
Module 4 - Pandas Challenge - Ryan Kincheloe

## Abstract
After combing through all the data pertaining to our students recent test scores, as well as the data about each individual school, there are some concerning trends we must address. 

First off, the students from charter schools out perform students the district schools by a large margin in both reading and math:

### Top 5 schools
![Top_schools](images/Top_schools.png)

### Bottom 5 schools
![Bottom_schools](images/Bottom_schools.png)

This leads me to believe our district schools are not teaching as effectively as the Charter schools. Effective teaching can be attributed to much more than the qualitty of teachers; including, but not limited to:
        - Student support resources
        - Quality of teaching materials
        - Program Resiliency (the ability of schools to continually adapt as the world changes and thus educational needs change)

I would recommend looking into the differences between the charter schools in the area and the district schools when it comes to curriculums, student materials & supplemental resources, and general educational/ school management philosophy. An external consultant might also provide insight into these areas. 


Secondly, it appears that the larger schools (2000-5000 students) typically perform worse than schools with fewer students. 

### Performance by school size 
![Performance_size](images/Bottom_schools.png)

These schools are almost entirely district schools (with the exception of Wislon High School) leads me to conclude that our schools are not equipped to handle the amount of students that attend. Teachers, administrators and resources are most likely spread too thin.



## Methodology
  This is the summary of my methods and steps taken to wrangle and analyze the data for our school district

- import dependencies
- setup connection to data
- read data files and store as a pandas dataframe
- merge datasets into single table
- calculate total number of unique schools
- calculate the number of students
- calculate total budget
- calculate mean math and reading scores
- Calculate percntage passing for each subject
- calculate overall passing percentage for all students
- initiate new data fram for required summary metrics district wide
- begin school summary section and group data by school
- establish the school summary as a dataframe
- set school as index and select school types
- create data frames for the best and worst performing schools
- display the top 5 schools and botttom 5 schools
- begin scores by grade section (repeat these steps for math and      reading scores)
    - separate data by grade
    - group by school and take mean of each
    - select only math/ reading scores
    - combine into a single data frame
    - display the data frame
- scores by school spending
- Create a copy of the school summary since it has the "Per Student Budget"
- ensure that per student budget is an integer not a string & remove formatting
- Use `pd.cut` to categorize spending based on the bins.
- Calculate averages for the desired columns.
- create new data frame for summary by school spending
- scores by school size
- establish bins
- categorize spending based on bins
- Use `pd.cut` on the "Total Students" column of the `per_school_summary` DataFrame.
- Calculate averages for the desired columns. 
- Create a DataFrame called `size_summary` that breaks down school performance based on school size (small, medium, or large).
- Use the scores above to create a new DataFrame called `size_summary`
- Display results
- scores by school type section
- Use the code provided to select new column data
- Assemble the new data by type into a DataFrame called `type_summary`
- Display results