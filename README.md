## Project II: Investigate a dataset
### * Udacity Data Analyst Nanodegree
### Table of contents
* [Setup](#setup)
* [Project Overview](#Project)
* [Data Wrangling](#Data_Wranging)
* [Data Cleaning](#Data_Cleaning)
* [Exploratory Data Analysis](#Exploratory_Data_Analysis)
* [Vizualization](#Vizualization)
* [Limitations](#Limitations)
* [Conclusion](#Conclusion)

## Setup
The project is created on Jupyter Notebook. The following packages are installed. These packages can be installed via conda or pip.
* Pandas
* Numpy
* Matplotlib
* Seaborn

## Project Overview - Investigate a dataset
In this project, I went through the data analysis process and saw how everything fits together.
I have used the Python libraries NumPy, pandas, and Matplotlib, which make writing data analysis code in Python a lot easier.
In my Data Analysis I explored the 'No-show appointments' data set. The data in the file contains records for people no shown for their appoitment.Patient information such as preexisting medical conditions and economic and social backgrounds has been given in the data set. The goal for this analysis is to find
the answer for the following questions using the exploratory analysis:
   1.People from which age group tends not to show up for their medical appointment and if there is any difference between male and female?
   2.Do people who participate in the Bolsa Família programe are more willing to show up for the appointment?
   3.Are people with preexisting medical conditions are more willing to missed their appointment?
In the project I have went through several steps - data wrangling, data cleaning amd exploratory data analysis where after the cleaning of the data I was able to find the answers of the listed questions and to make conclusions.

## Data Wrangling
In this part I have investigate the chosen dataset which is attached in the project.The dataset contains information for people who are not showing for their appointments.I have read the file,creating a dataframe,showing the shape of the dataset and find the datatypes of each column.

## Data Cleaning
Based on the previous investigations I was able to do a data cleaning in this part of the project. I have renamed the existing columns to more readable names and converted them to lowercase. I have also changed the wrong datatypes. I got rid of the wrong records( ex: people with negative age) using the clip() function to trim values at input threshold(0,95). I have creaetd a new column named 'age group' using bin to group people in common age groups. I have shifhted formward with 1 day the appointment day because in some records the scheduled day was after the appointment day.

## Exploratory Data Analysis
In this part of the project I have observed the listed questions using different pandas functions.I have used groupby function to group people into groups and to make some findings about the dataset.I have created a custom function to plot no show rate by age groups across other variables in order to avoid repetitive code.

## Vizualizations
To ansswer the 1st question I have used a bar chart to describe number of no shows across age groups and line chart to describe number of no shows across age groups and gender.
To answer the 2nd question  I have used a bar chart to express no show rate by age groups across scholarship.
To answer the 3rd question I have used a line chart to expressno show rate by age groups across different preexisting diseases- diabetes, hypertension,alcoholism.

## Limitations
Despite the fact that there were no null values in the data set there were a bunch of iconsistent data. In the age column some of the rows were equal to -1 which is irrelevant - you can not be on negative age so I was forced to drop all the rows where the age was -1. Also there was a misconsistence between the appointment and scheduled day so I had to shift the appointment day with one day foreward. After a plenty of data cleaning I came up with a more appropriate data set in which I could made some conclusions about my findings.
## Conclusion
After the analysis that I have done I came up with several findings:

With age people tend to attend more their appointments and people from age group 13-17 are missing their appointments the most.
Gender doesn't affect people's decision about showing for the appointment or not.
People who participate in the schoolarship programme are more willing to miss their appointments.
People who suffer from any disease are more willing to show for their apointment.
When I explored the no show rate by age I found that people from age group(18 to 24) who have diabetes and hypertension have the highest rate of no shows.
