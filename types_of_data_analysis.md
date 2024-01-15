# Types of Data Analytics
![image](https://github.com/heiditm/heiditm.github.io/assets/56846204/8b252ebf-79de-4295-91f3-cfa1665d5ccc)
**There are two main types of analytics:** 
  -  **Reactive Analytics**, which is used to understand the data in its current and historical state – more commonly divided into *descriptive* and *diagnostics* analysis.
  -  **Proactive Analytics**, which uses the data to forecast/predict a future event and recommends an action to be taken – more commonly divided into *predictive* and *prescriptive* analysis.
  -  <span style="color: #228B22"> **Example:** </span> To illustrate the different results provided by each analysis we will center around an example regarding airline data (imagine this dataset consist of **dates, sales, airports and gasoline prices** for our current purposes).

<code style="color : #228B22"> **Reactive Analysis** </code> aims to understand what is happening in the data and why it is happening in its current and historical state.  

<span style="color:#3498DB"> **Descriptive Analysis** </span> is used to describe what is happening in the raw data. It does not make assumptions to the data but is strictly used to review what really happen in the data. Some measures taken in this analysis are: 
- **Distribution:** Understanding the distribution of data by looking at the quartiles, percentiles or frequencies *(Ex: Box plot)*
- **Central Tendencies:** Understanding where the center of the data lies *(Ex: Mean, Median, Mode)*
- **Variability:** Understanding how the data is spread out *(Ex: standard deviation, variance, range)*

    <span style="color:forestgreen"> **Example:** </span>  Current annual data shows an increase in gasoline prices compared to the prior year. 

<span style="color:#3498DB"> **Diagnostic Analysis** </span> is used to understand why the data happened the way it did. Its main goal is to find the cause and effects of the situation. Diagnostic analysis usually involves comparing datasets or variables to find connections or relationships by identifying **correlations, filtering** data and/or performing **univariate/bivariate or multivariate** analysis.  One thing to always remember is that: correlation does not imply causation. 

<span style="color:forestgreen"> **Example:** </span>  Historical data shows high demand/sales from LA  NYC pre-Christmas holiday. 

<span style="color:orange"> **Exploratory Data Analysis** </span> - The measures used in descriptive and diagnostics analysis are a part of exploratory data analysis (EDA). Exploratory data analysis aims to figure out the what and whys of the data through measures and visualizations mentioned above as well as attempt to identify any **abnormalities, errors, trends, detect outliers and interesting relationships**. It can also **check assumptions, test hypothesis** and may help **identify potential algorithms used for proactive analysis.**  

<span style="color:forestgreen"> **Proactive Analysis** </span> aims to forecast and predict future events using the data for improvements and developments. 

<span style="color:#3498DB"> **Predictive Analysis** </span>  uses modeling techniques to forecast predictions to find the likelihood of an event happening and is used to evaluate a decision. Predictive analysis usually uses findings and insights from reactive analysis to spot common outcomes and discover causes. By using statistical modeling techniques, it helps understand the consequences of a decision based on the predictions on how variables will act and perform. 

<span style="color:forestgreen"> **Example:** </span>  A machine learning algorithm learns through the detected trend of high demands from LA  NYC preChristmas holiday and forecast its predictions for the current year. Results show that there are less sales this year pre-Christmas holiday in comparison to the prior year in its projected state. 

<span style="color:#3498DB"> **Prescriptive Analysis** </span>  uses the outcomes from the predictive analysis and recommends an effective action to be taken, with artificial intelligence (AI) these results could be provided in real-time.  

<span style="color:forestgreen"> **Example:** </span>  As a possible result an airline may (automatically with AI) lower the prices of tickets to a threshold price while accounting for the increase in gasoline prices (and/or miscellaneous factors). 

<span style="color:orange"> **ALGORITHM/AI/ML/DL** </span> - Predictive and Prescriptive analysis usually works together as they will both involve statistical modeling techniques or tools to understand and deep dive into the data.  
- **Algorithms:** Specific statistical modeling techniques or algorithms needed based on the data or research question
- **Artificial Intelligence/Machine Learning/Deep Learning:** Linear Regression, Random Forests, Clustering, Neural Networks, Pattern Recognition, etc. 



















<!--
Here we will explore the  [**Early Classification of Diabetes**](https://www.kaggle.com/datasets/andrewmvd/early-diabetes-classification/data) dataset through exploratory data analysis (EDA) and predictive analysis (Classification).

**Time Frame Conducted:** Unknown, prior to 2019  
**Location:** Sylhet Diabetes Hospital in Sylhet, Bangladesh  
**Research Question:** What are the early signs of diabetes? What is the best machine learning technique to accuracy predict and classify a patient has diabetes?

**Synopsis of Study:** This data was collected through direct questionnariess and diagnosis results from newly affected patients who have signs and symptoms of diabetes.

This dataset consists of 520 observations and 17 variables:
- Dataset values description:
  - 1 = Yes
  - 0 = No

Variable|Description
-|:---
Age|Age of patient (16-90).
Gender|Gender of patient.
Polyuria|Excessive urination volume, considered usually if more than 2.5 liters per day.
Polydipsia|Excessive thirst, one of the first symptoms of diabetes
Sudden Weight Loss|A significant drop in weight without a change in diet or exercise. Can occur in people with type 2 diabetes but more common with type 1.
Weakness|Feeling of fatigue.
Polyphagia|Excessive hunger that increases appetite significantly and persistently. One of the main symptoms of diabetes.
Genital Thrush|A yeast infection, high sugar levels supply better conditions for infection to grow.
Visual Blurring|Loss of sharpness of vision and makes it impossible to see fine details. Instability of blood sugar is known to be the reason for blurred vision.
Itching|Irritation to the skin.
Irritability|Feeling of agitation and anger as a result of stress.
Delayed Healing|Taking longer to heal than normal.
Partial Paresis|Weakness of voluntary movement, can be a symptom of diabetes.
Muscle Stiffness|The inability of the muscles to relax normally. It can affect any part of the body and causes difficulty of moving.
Alopecia|Leads to hair loss on any part of the body.
Obesity|Having excess body fat.
Class|Diagnosis with diabetes. <br>1 Positive <br>0 Negative

**Class**|**Summary Percentage**
-|-
Positive|61.54%
Negative|38.46%

**Sex**|**Summary Percentage**
-|-
Male|63.10%
Female|36.92%

**Diabetes** is a chronic disease that affects how the human body turn food into energy. Currently there is no cure for diabetes but losing weight, being active and eating healthy can help.

Normally the body breaks down majority of the food taken into sugar/glucose and releases into the bloodstream. If blood sugar increase it signals the pancreas to release insulin. Insulin acts as a key to let the blood sugar into the body's cells to use as energy.

Diabetes is when the body does not make enough insulin or use it as well as it should. When this happens there is a blockage/buildup of blood sugar in the bloodstream which can cause serious health problems such as heart disease, vision loss or kidney disease.

There are 3 types of diabetes:

**Type 1 Diabetes: 5% - 10%**
- Theoretically caused by an autoimmune reaction where the body attacks itself by mistake. This reaction will stop the body from making insulin. This type can be diagnosed at any age and symptoms often develop quickly. Patients who are diagnosed with Type 1 will have to take insulin daily for life to survive. Currently there is no way to prevent Type 1 diabetes.

**Type 2 Diabetes: 90% - 95%**
- The body does not use insulin well and blood sugar levels cannot keep at normal levels. It develops over many years and will usually be diagnosed in young adults. Symptoms may not be noticeable so it is recommended to test blood sugar levels if you are at risk.
  - **Prediabetes**
    - In the United States, more than 1 in 3 people has prediabetes and more than 8 in 10 do not know they have it. With prediabetes, blood sugar levels are higher than normal but is not enough to be diagnosed as Type 2. Prediabetes will also raise the risk for heart disease and stroke.

**Gestational Diabetes: Pregnant Women who never had diabetes**
- If diagnosis with this, the baby could have higher risk of health problems. Gestational diabetes usually goes away after the baby is born, however it increases the risk of the mom for Type 2 diabetes later in life. The baby is more likely to have obesity as a child or teen and develop type 2 diabetes later in life.

![diabetes countplots](https://github.com/heiditm/heiditm.github.io/assets/56846204/865ace74-b5dd-4f38-9f64-d947d6f3191d)

Early symptoms of diabetes (sorted from highest likelihood):

Variable|50% of Male patients fall between ages|50% of Female patients fall between ages|Note
-|:-:|:-:|-
Polydipsia|47 - 58|39 - 55|All female patients with polydipsia was diagnosed with diabetes.
Polyuria|44 - 60|39 - 55|All female patients with polyuria was diagnosed with diabetes.
Sudden Weight Loss|48 - 58|39 - 55
Partial Paresis|54 - 66|39 - 55
Visual Blurring|52 - 62|39 - 55
Weakness|47 - 61|39 - 54
Itching|41 - 60|39 - 55

![diabetes boxplot](https://github.com/heiditm/heiditm.github.io/assets/56846204/252d6aa8-5b2f-4b89-a15a-65a496fe12f4)

We will try to find the best method to predict and classify diabetes with our data using logistic regression, decision tree, k nearest neighbors and support vector machines.

![diabetes confusion matrix](https://github.com/heiditm/heiditm.github.io/assets/56846204/a90db023-4962-4d2c-af8c-4f51fba5b11d)

Method|Accuracy %
-|-
Decision Tree|	98.0769
Support Vector Machines|	95.1923
K Nearest Neighbors|	94.2308
Logistic Regression|	91.3462

The decision tree method shows the best accuracy to predict and classify diabetes with the variables in our data. Support vector machines and K nearest neighbors are very similar in accuracy, falling behind decision tree. Logistic regression shows to be the least accurate classifier, wrongly predicting 9 patients.


<!--
**Insights:**
- Survival rates starts to show significant increase after 4+ years
- Age is unlikely a potential factor although patients over the age of 73 show to have less than a 45% survival rate
- The presence of an ulceration shows to have 50% survival rate
- The absence of an ulceration shows to have around an 85% survival rate
- Survival rates are about 80% for Young Adults and Middle Aged patients while around 60% in Children and Seniors patients
- Male survival rate is about 60%
- Female survival rate is over 75%
- Larger thicknesses show a higher probability of a presence of an ulceration
- Thicknesses larger than 3.54mm have about an average survival rate of 44%

### Takeaways | Answer to Research Question shows:
Yes, both thickness and presence of a ulcerated tumor increases the chance of death from malignant melanoma.

- Females are twice as likely to survive than males
- The first 4 years are the most crucial (majority of deaths occur between 2 - 4.5 years with an average of 3.5 years)
- Essentially it becomes more crucial with age
- Factors that **worsen chances of survival** are:
  - Larger thicknesses (over 3.54mm have about an average survival rate of 44%)
  - The presence of an ulceration (survival rates drop to 50/50, regardless of sex)
    - **Note:** Larger thicknesses shows a higher probability in the formation of an ulceration-->
