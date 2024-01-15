# Types of Data Analytics
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/8b252ebf-79de-4295-91f3-cfa1665d5ccc)
**There are two main types of analytics:** 
  -  **Reactive Analytics**, which is used to understand the data in its current and historical state – more commonly divided into *descriptive* and *diagnostics* analysis.
  -  **Proactive Analytics**, which uses the data to forecast/predict a future event and recommends an action to be taken – more commonly divided into *predictive* and *prescriptive* analysis.
  -  <b code style="color: forestgreen"> Example: </b> To illustrate the different results provided by each analysis we will center around an example regarding airline data (imagine this dataset consist of **dates, sales, airports and gasoline prices** for our current purposes).

<b code style="color: forestgreen"> Reactive Analysis </b> aims to understand what is happening in the data and why it is happening in its current and historical state.  

<b code style="color : dodgerblue "> Descriptive Analysis </b> is used to describe what is happening in the raw data. It does not make assumptions to the data but is strictly used to review what really happen in the data. Some measures taken in this analysis are: 
- **Distribution:** Understanding the distribution of data by looking at the quartiles, percentiles or frequencies *(Ex: Box plot)*
- **Central Tendencies:** Understanding where the center of the data lies *(Ex: Mean, Median, Mode)*
- **Variability:** Understanding how the data is spread out *(Ex: standard deviation, variance, range)*

&ensp; <b code style="color : forestgreen"> Example: </b> Current annual data shows an increase in gasoline prices compared to the prior year. 

<b code style="color : dodgerblue "> Diagnostic Analysis </b> is used to understand why the data happened the way it did. Its main goal is to find the cause and effects of the situation. Diagnostic analysis usually involves comparing datasets or variables to find connections or relationships by identifying **correlations, filtering** data and/or performing **univariate/bivariate or multivariate** analysis.  One thing to always remember is that: correlation does not imply causation. 

&ensp; <b code style="color : forestgreen"> Example: </b>  Historical data shows high demand/sales from LA to NYC pre-Christmas holiday. 

<b code style="color : darkorange"> Exploratory Data Analysis </b> - The measures used in descriptive and diagnostics analysis are a part of exploratory data analysis (EDA). Exploratory data analysis aims to figure out the what and whys of the data through measures and visualizations mentioned above as well as attempt to identify any **abnormalities, errors, trends, detect outliers and interesting relationships**. It can also **check assumptions, test hypothesis** and may help **identify potential algorithms used for proactive analysis.**  

<b code style="color: forestgreen"> Proactive Analysis </b> aims to forecast and predict future events using the data for improvements and developments. 

<b code style="color : dodgerblue "> Predictive Analysis </b>  uses modeling techniques to forecast predictions to find the likelihood of an event happening and is used to evaluate a decision. Predictive analysis usually uses findings and insights from reactive analysis to spot common outcomes and discover causes. By using statistical modeling techniques, it helps understand the consequences of a decision based on the predictions on how variables will act and perform. 

&ensp; <b code style="color : forestgreen"> Example: </b>  A machine learning algorithm learns through the detected trend of high demands from LA to NYC preChristmas holiday and forecast its predictions for the current year. Results show that there are less sales this year pre-Christmas holiday in comparison to the prior year in its projected state. 

<b code style="color : dodgerblue ">  Prescriptive Analysis </b> uses the outcomes from the predictive analysis and recommends an effective action to be taken, with artificial intelligence (AI) these results could be provided in real-time.  

&ensp; <b code style="color : forestgreen">Example: </b>  As a possible result an airline may (automatically with AI) lower the prices of tickets to a threshold price while accounting for the increase in gasoline prices (and/or miscellaneous factors). 

<b code style="color : darkorange"> ALGORITHM/AI/ML/DL </b> - Predictive and Prescriptive analysis usually works together as they will both involve statistical modeling techniques or tools to understand and deep dive into the data.  
- **Algorithms:** Specific statistical modeling techniques or algorithms needed based on the data or research question
- **Artificial Intelligence/Machine Learning/Deep Learning:** Linear Regression, Random Forests, Clustering, Neural Networks, Pattern Recognition, etc. 
