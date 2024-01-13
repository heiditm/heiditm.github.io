# Early Classification of Diabetes
Analysis Written By: Heidi

Here we will explore the  [**Early Classification of Diabetes**](https://www.kaggle.com/datasets/andrewmvd/early-diabetes-classification/data) dataset through exploratory data analysis (EDA) and predictive analysis (Classification).

**Time Frame Conducted:** Unknown, prior to 2019  
**Location:** Sylhet Diabetes Hospital in Sylhet, Bangladesh  
**Source:** Kaggle  
**Research Question:** What are the early signs of diabetes?

**Synopsis of Study:** This data was collected through direct questionnariess and diagnosis results from newly affected patients who have signs and symptoms of diabetes.

This dataset consists of 520 observations and 17 variables:
- In the dataset the values mean:
  - 1 Yes
  - 0 No

Variable|Description
-|:---
Age|Age of patient (16-90)
Gender|Gender of patient
Polyuria|Excessive urination volume, considered usually if more than 2.5 liters per day.
Polydipsia|Excessive thirst, one of the first symptoms of diabetes
Sudden Weight Loss|A significant drop in weight without a change in diet or excercise. Can occur in people with type 2 diabetes but more common with type 1.
Weakness|Feeling of fatigue.
Polyphagia|Excessive hunger that increases appetite significantly and persistently. One of the main symptoms of diabetes.
Genital Thrush|A yeast infection, high sugar levels supply better conditions for infection to grow.
Visual Blurring|Loss of sharpness of vision and makes it impossible to see fine details. Instability of blood sugar is known to be the reason for blurred vision.
Itching|Irritation to the skin.
Irritability|Feeling of agitation and anger as a result of stress.
Delayed Healing|Taking longer to heal than normal.
Partial Paresis|Weakness of voluntary movement, can be a symptom of diabetes.
Muscle Stiffness|The inability of the muscles to relax normally. It cn affect any part of the body and casues difficulty of moving.
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

Normally the body breaks down majority of the food taken into sugar/glucose and releases into the bloodstream. If blood sugar increase it signals the pancreas to release insulin. Insulin acts as a key to let the blood sgar into the body's cells to use as energy.

Diabetes is when the body does not make enough insulin or use it as well as it should. When this happens there is a blockage/build up of blood sugar in the bloodstream which can cause serious health problems such as heart disease, vision loss or kidney disease.

There are 3 types of diabetes:

**Type 1 Diabetes: 5% - 10%**
- Theoretically caused by an autoimmune reaction where the body attacks itself by mistake. This reaction will stop the body from making insulin. This type can be diagnosed at any age and symptoms often develop quickly. Patients who are diagnosed with Type 1 will have to take insulin daily for life to survive. Currently there is no way to prevent Type 1 diabetes.

**Type 2 Diabetes: 90% - 95%**
- The body does not use insulin well and blood sugar levels cannot keep at normal levels. It develops over many years and will usually be diagnosed in young adults. Symptoms may not be noticeable so it is recommended to test blood sugar levels if you are at risk.

**Gestational Diabetes: Pregnant Women who never had diabetes**
- If diagnosis with this, the baby could have higher risk of health problems. Gestational diabetes usually goes away after the baby is born, however it increases the risk of the mom for Type 2 diabetes later in life. The baby is more likely to have obesity as a child or teen and develop type 2 diabetes later in life.


![diabetes countplots](https://github.com/heiditm/heiditm.github.io/assets/56846204/865ace74-b5dd-4f38-9f64-d947d6f3191d)

### Early symptoms of diabetes (sorted from highest likelihood):
- Polydipsia
- Polyuria
- Irratability
- Sudden Weight Loss
- Partial Paresis
- Polyphagia
- Visual Blurring
- Weakness
- Itching


<!---<img src="images/melanoma boxplot.png"/>

- A critical time frame of 5 years based on the status of the patients for all stages (which matches the initial research for the survival rates)

<img src="images/melanoma 1.png"/>

- Female patients are twice as likely to live through melanoma than male patients
- Presence of an ulceration show survival rates to be 50 - 50 regardless of sex
- Patients are 5.7 times more likely to survive if they do not show ulceration


<img src="images/melanoma 2.png"/>

- In general, regardless of sex, patients without ulceration have a better chance of survival (with females having a higher likelihood) whereas patients with an ulceration seem to have a 50 - 50 chance of survival
- Females without ulceration are 8.5 times likely to survive
- Males without ulceration are 3 times more likely to survive
- Essentially it becomes more crucial with age

<img src="images/melanoma bubble.png"/>

- Most deaths occur in patients with an ulceration and larger thicknesses
- Patients without an ulceration generally have a smaller thickness

<img src="images/melanoma crossplot 1.png"/>
<img src="images/melanoma crossplot 2.png"/>
<img src="images/melanoma crossplot 3.png"/>
<img src="images/melanoma crossplot 4.png"/>
<img src="images/melanoma crossplot 5.png"/>
<img src="images/melanoma crossplot 6.png"/>
<img src="images/melanoma crossplot 7.png"/>

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
