# Data-Analysis-on-health-outcomes-and-preventive-services-in-the-United-States-

‘PLACES’ is the state-of-the-art health dataset funded by the Centers for Disease Control (CDC) and the Robert Wood Johnson Foundation. This dataset only used to exist for the 500 largest cities in the United States, but has been expanded to county resolution. The purpose of the dataset is to provide estimates of chronic disease risk factors, health outcomes, and clinical preventive service use in the United States. These estimates will allow cities and local health departments to better understand the burden and geographic distribution of health-related variables in their jurisdictions and assist them in planning public health interventions.

Source for the original data: https://www.cdc.gov/places/index.html 
Link to the clean dataset (cleaned and curated for you): https://drive.google.com/file/d/11lH8PWlAzD9kGOBPQ1ffM4yusU-y2pcO/view?usp=sharing 
Data dictionary: The dataset includes estimates for 27 measures: 5 chronic disease-related unhealthy behaviors, 13 health outcomes, and 9 on use of preventive services. They are listed in this data dictionary: https://docs.google.com/spreadsheets/d/12vMGi1rShBCv9kg_LdRx7S-04eqqc5_q/edit?usp=sharing&ouid=115978987638220839052&rtpof=true&sd=true 


#Exploratory Data Analysis 
Explore the data by geography!

The PLACES cities data encompasses 1) ‘Use of preventative services’, 2) ‘unhealthy behaviors’ and 3) ‘health outcomes’ and you now have data on regions and divisions. Make five interesting tables and five interesting plots. Make sure each plot and table is LABELED and has a descriptive caption. 

Using the exploratory data analysis you’ve conducted, select ONE ‘health outcome’ (like ALL TEETH LOST, ARTHRITIS… or STROKE) which you will use for modeling. You can find a list of health outcomes in the data dictionary: https://docs.google.com/spreadsheets/d/12vMGi1rShBCv9kg_LdRx7S-04eqqc5_q/edit?usp=sharing&ouid=115978987638220839052&rtpof=true&sd=true 

#Literature Review 
Using your selected health outcome, go read at least 10 scientific articles, blogs, news stories etc. and say something about the ‘health outcome’ you have selected - give a high-level overview in the form of a literature review. What are the current trends? Is it preventable? Does it affect a certain community/demographic? Is there new medication available? Has the pandemic affected the incidence?

#Hypothesis Testing 
Conceptualize and design a) one sample and b) two-sample hypothesis test. Compute by hand like we do in class (with a graph of the test statistic and critical value on a graph), write LaTeX formulas for the test statistic, calculate the p-value and say what the results of the test mean in plain English. 10 pts for each test. 


#Modeling and Error Metrics

Regression
Linear - full variables
Use all the variables that make sense to predict your health column (don’t use the FIPS column or ID columns!) Just use the health outcomes, prevention and unhealthy behaviors data.
Store your predictions in a vector for use later. 
Calculate AIC, RMSE, MAE, scatterplot of actual vs. predicted with nice titles/labels, and any other metrics that you want to analyze.
Linear - reduced variables
Use stepwise forward, backwards regression or p-hacking.
Store predictions in a vector for use later.
Calculate AIC, RMSE, MAE, scatterplot of actual vs. predicted, and any other metrics.

Classification
Now, create a new column called ‘Flag’ for your ONE health outcome variable. Make it a ‘1’ if the row has a value GREATER than the median. Make it a ‘0’ if it is less than or equal to the median value. Now you will fit a LOGISTIC REGRESSION for your health outcome. 

Logistic - full variables
Use all the variables that make sense. Don’t use your original health outcome to predict the flag variable - this is data leakage!
Store your 0/1 predictions in a vector for use later. 
Calculate AIC, confusion matrix, accuracy, TPR, TNR, FPR, FNR
Logistic - reduced variables
Use stepwise forward or backwards regression.
Store 0/1 predictions in a vector for use later. 
Calculate AIC, confusion matrix, accuracy, TPR, TNR, FPR, FNR


Conclusion
Wrap it up and say something about health in the United States and any next steps you would be interested in pursuing in the future. Be creative and generalize about your conclusions, talk about the value of your analysis. Make sure your ‘works cited’ page is at the end of your document.
