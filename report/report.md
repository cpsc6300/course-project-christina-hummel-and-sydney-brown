

# TITLE: Socioeconomical Impacts on Healthcare Access Trends
## Team Members: Sydney Brown and Christina Hummel
## Date: 12/10/2020

# Probelm Statement and Motivation
This should be a brief and self-contained decription of the problem that your project aims to solve and what motivated you to solve this problem.

As bioengineering students, we are passionate about the intersection of data science and healthcare. For this project, our particular interests surround the investigation of healthcare data to determine how demographic variables such as race, gender, and household income play a role in influencing access to care by looking at variables such as private insurance information, default care location/source, and primary healthcare provider. In addition, we would like to predict the number of times an individual receives care per year based on inputs such as income, health condition, routine place of care, and insurance. 

# Introduction and Description of Data
Description of relevant knowledge. Why is this problem important? Why is it challenging? Introduce the motivations for the project question and how that question was defined through preliminary EDA.

Based on the current state of the world and the struggle to combat the COVID-19 pandemic, it is clear that improvements can be made to the healthcare system as a whole and that access to healthcare is not equal across the board. Through the use of publicy available datasets, it is our revised goal to analyze information surrounding the general health and well-being of subjects in hopes to analyze how certain factors including insurance, demographic variables, and typical practices for receiving healthcare relate to overall access to care. After some initial investigation and searches through publically available datasets, we hope to investigate how access to health care and insurance is affected by occupation and income and how racial background may be correlated to this access and assistance. The dataset we chose to use for our investigation is publicly provided through the Center for Disease Control. The CDC conducts the National Health and Nutritional Examination Survey yearly and publishes the raw data that contains a significant amount of information with many categorical variables about demographics and access to care to aid us in this mission. Within the 2013-2014 NHANES dataset, we specifically used the demographics and questionnaire sub-datasets for this project. 

# Literature Review/Related Work 
This could include noting any key papers, texts, or websites that you have used to develop your modeling approach, as well as what others have done on this problem in the past. You must properly credit sources.

CDC NHANES Documentation [1]:
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/HUQ_H.htm
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/DEMO_H.htm
We used this documentation extensively in our work. The NHANES documenation gave us extensive background on what the survey is, how it was collected, and what types of information are stored in it. The demographic and questionnaire documentation specifically provided the codes in the datasets that we needed in order to determine column headers and meanings of value codes. 

Literature Review for the Problem Statement:
First, we hoped to gain an understanding on how the average American accessed healthcare, and we found that 84.3% of adults and 93.6% of children had contact with a healthcare professional in the past year, and on average, people visited a physician 2.7 times per year [2].
We also reviewed literature on studies published on how demographics influence access to healthcare in the US, especially how this relates to race and income. A literature review on healthcare for low income families revealed that key barriers to adequate care are a lack of education, health insurance complications, and an overall distrust of health care providers [3]. Another explored race and healthcare by studying how the community that Hispanics live in impacts their access to healthcare. The results showed that access to care was negatively associated with Mexican Americans who did not have insurance and were living in areas more heavily populated with Spanish-speaking immigrants [4]. With our investigation, we sought to support results like these using the NHANES dataset. 



# Modeling Approach

+ Describe the baseline model.
+ Describe your implementations beyond the baseline model and the design choices that you have made.

We decided to use a DecisionTree Classifier as our baseline predictive model. The target variable is the number of care received per year per individual. The target variable includes 8 categories, breaking the number of visits per year into ranges from 0 to 16 times per year. The feature variables are income, health insurance, general health condition, routine place for healthcare, and whether a mental health doctor is visited. Because the DecisionTree was so large and to avoid over-fitting, we made the decision to prune the tree using a max depth. We ran the model multiple times using max depths up to 8 and found that the accuracy only slightly increased, so we settled on a max depth of __.


# Project Trajectory, Results, and Interpretation 

Briefly summarize any changes in your project goals or implementation plans you have made.
These changes are a natural part of any project, even those that seem the most straightforward at the beginning.
The story you tell about how you arrived at your results can powerfully illustrate your process. 

Initially, our main goal for the project was to predict how demographic information about an individual might predict their access to care. We began by cleaning the data, which was a more arduous task than anticipated. We needed to find and replace coded values in the data that represented that the individual did not know or refused to answer the question in order to prevent these values skewing the data. The initial data was integer encoded, so we replaced the encoded integers with their meaning in order to enhance and provide meaning to visualizations. We then created many visualizations in order to visually see the effect of demographic variables on each other and on the healthcare and insurance information. From these visualizations, it was clear that income was the main influential variable in terms of healthcare and insurance, and we decided to move forward with income as the only demographic variable used in our predictive model. As we worked through the data, we realized there was no clear target variable for a model that would embody access to care. Because of this, the final predictive model demonstrates how income, insurance, type of routine place visited for care, mental health care, and overall health condition impact and help predict the number of times an individual receives care in a particular year.

Next, show your results. How well does your model and/or implementation perform? Did you meet your goals?

Finally, give some interpretation. What do your results mean? What impact will your work have?

# Conclusions and Future Work
Summarize your results, the strengths and short-comings of your results, and speculate on how you might address these short-comings if given more time.

# References:
This could include the revised key papers, texts, or websites that you may use to develop your project.

[1] https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/HUQ_H.htm
https://wwwn.cdc.gov/Nchs/Nhanes/2013-2014/DEMO_H.htm
[2] "Ambulatory Care Use and Physician office visits." The Center for Disease Control and Prevention, 2019. https://www.cdc.gov/nchs/fastats/physician-visits.htm
[3] Lazar M, Davenport L. Barriers to Health Care Access for Low Income Families: A Review of Literature. J Community Health Nurs. 2018 Jan-Mar;35(1):28-37. doi: 10.1080/07370016.2018.1404832. PMID: 29323941.
[4] Gresenz, Carole Roan, et al. “Community Demographics and Access to Health Care among U.S. Hispanics.” Health Services Research, Blackwell Science Inc, Oct. 2009, www.ncbi.nlm.nih.gov/pmc/articles/PMC2754547/. 

# Support Materials
Provide a list of materials that support your project, for example, the notebooks and data sources.

# Declaration of academic integrity and responsibility

In your report, you should include a declaration of academic integrity as follows:

```
With my signature, I certify on my honor that:

The submitted work is my and my teammates' original work and not copied from the work of someone else.
Each use of existing work of others in the submitted is cited with proper reference.
Signature: ____________ Date: ______________
```

# Credit
The above project template is based on a template developed by Harvard IACS CS109 staff (see https://github.com/Harvard-IACS/2019-CS109A/tree/master/content/projects).
