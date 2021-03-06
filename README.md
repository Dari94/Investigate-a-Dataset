## Project II: Investigate a dataset
### * Udacity Data Analyst Nanodegree
### Table of contents
* [Setup](#setup)
* [Project Overview](#Project)
* [Data Wrangling](#Data_Wranging)
* [Data Cleaning](#Data_Cleaning)
* [Exploratory Data Analysis](#Exploratory_Data_Analysis)
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
Statistics were computed to find out the probabilities of converting regardless of page. These were used to analyze if one page or the other led to more conversions.

## Data Cleaning
The A/B testing was conducted assuming the old page is better unless the new page proves to be definitely better at a Type I error rate of 5%. The data was bootstrapped and sampling distributions were determined for both pages. Conclusions were drawn on conversions for both pages by calculating p-values.

## Exploratory Data Analysis
Logistic regression was then performed to confirm results of the previous steps. Null and alternative hypotheses associated with this regression model were stated and verified using statsmodel.

## Conclusion
Based on the statistical tests I used, the Z-test, logistic regression model, and actual difference observed, the results have shown that the new and old page have an approximately equal chance of converting users. We fail to reject the null hypothesis. Overall there is not enough evidence on deciding to switch to the new page rather than stay with the old one so I recommend to the e-commerce company to keep the old page.
