# TITLE: Social, Economical, and Geographical Impacts on Healthcare Access Trends
## Team Members: Christina Hummel and Sydney Brown
## Date: 11/12/2020

# Project Description
## Probelm Statement and Motivation
This should be a brief and self-contained decription of the problem that your project aims to solve and what motivated you to solve this problem.

As bioengineering students, we are passionate about the intersection of data science and healthcare. For this project, our particular interests surround the investigation of healthcare data to determine how demographic variables such as race, gender, household income, and age play a role in influencing access to care by looking at variables such as private insurance information, default care location/source, and primary healthcare provider. 

## Introduction and Description of Data
Description of relevant knowledge. Why is this problem important? Why is it challenging? Introduce the motivations for the project question and how that question was defined through preliminary EDA.

Based on the current state of the world and the struggle to combat the COVID-19 pandemic, it is clear that improvements can be made to the healthcare system as a whole. Through the use of publicy available datasets, it is our revised goal to analyze information surrounding the general health and well-being of subjects in hopes to analyze how certain factors including access to care, insurance, and demographic variables relate to overall health. After some initial investigation and searches through publically available datasets, we now hope to investigate topics such as how access to health care and insurance is affected by occupation and income, how racial background may be correlated to this access and assistance, and how age and gender correlates to certain disease states. Following further investigations, we were able to find subsequent data within the inital data set through the Center for Disease Control and the National Health and Nutritional Examination Survey that contains a significant amount of information with many categorical variables about demographics and access to care to aid us in this mission.


## Literature Review/Related Work 
This could include noting any key papers, texts, or websites that you have used to develop your modeling approach, as well as what others have done on this problem in the past. You must properly credit sources.

https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/HUQ_H.htm
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/DEMO_H.htm

We have needed to use these sites extensively in our preliminary work. The CDC website gave us a lot of background on what this survey is, how it was collected, and what types of information are stored in it. The site gives us the codes that are column names in the datasets that we needed in order to figure out what we were looking at in the data. 

We have also reviewed some literature on studies that people have already done on how demographics influence access to healthcare in the US, especially how this relates to race. One particularly interesting study explored how the community that Hispanics live in impacts their access to healthcare.

## Interim Results
If you have some interim results or new findings, you can include them here.

At this point in working through this project, we were able to download the initial datasets and visualize them within a Jupyter notebook. The National Health and Nutrition Examination Survey has an extensive codebook to outline all of the keyed column names, so we did extensive reading about the codes in order to determine which columns in the data were the best fit for our project mission. Once we decided which columns within the datasets we wanted to work with, we narrowed our dataframes within Python to reflect this change and continued on with data cleaning tasks, such as removing null values and outliers and also assigning value to categorical variables. 

# Project Progress
This could include the __revised__ major timeline and milestones of your project as well as requirements of computing and storage resources. 

This may also include a brief summary of your team's progress on the project and a candid reflection of what's gone wrong and what's gone right, and what efforts that your team have taken or are going to takea to overcome any issue that comes out during the course of the project.

Total: 7 weeks to completion

Week 1-3:

Source a data set(s) that give information regarding prevelance of disease, cause of death, and quality of care in reference to geograhpical location
Download dataset into Jupyter notebook and establish workspace
Work to clean and compile the dataset

Weeks 3&4:

Get rid of null values
remove outliers
Assign value to categorical variables
Analyze the data and determine best modes for visualization
Create visuals to communicate final insights from data analysis

Weeks 5-7:

Create predictive indexes for specific demographics (i.e age, gender, race)
Create website to showcase the final analysis and insights

Initially, we really struggled in finding publicly available data related to healthcare, but we persisted and believe that the National Health and Nutrition Examination Survey gives us the information we need to be sucessful. We also spent a fair amount of time figuring out how to load the dataset into our jupyter notebook: initially we were trying to use a direct URL from the website but later learned that we had to download the csv into our github repository in order to get a successful .csv link that would work in Python. We now feel comfortable moving forward, as we have narrowed down the data so it isn't so intimidating, and we have a clear path of how we want to move forward based on our past assignments doing similar work.

# References:
This could include the revised key papers, texts, or websites that you may use to develop your project.
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/HUQ_H.htm
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/DEMO_H.htm

Gresenz, Carole Roan, et al. “Community Demographics and Access to Health Care among U.S. Hispanics.” Health Services Research, Blackwell Science Inc, Oct. 2009, www.ncbi.nlm.nih.gov/pmc/articles/PMC2754547/. 
