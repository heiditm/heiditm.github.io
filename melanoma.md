## Malignant Melanoma - Variables that Increase Chance of Death

Here we will explore the [Melanoma](https://stat.ethz.ch/R-manual/R-devel/library/boot/html/melanoma.html) dataset through exploratory data analysis (EDA).

**Time Frame Conducted:** 1962 - 1977 <br>
**Location:** Department of Plastic Surgery, University Hospital of Odense, Denmark <br>
**Research Question:** Does thickness and/or ulcerated tumors have an increase chance of death from malignant melanoma?

**Synopsis of Study:** Measurements were made on patients with malignant melanoma with each patient's tumor removed. During the surgery the tumor is removed with around 2.5cm of the surrounding skin. Measurements of thickness and ulcerated presence were taken as these variables were predicted to increase the chance of death from the disease. Patients were followed until the end of 1977.

This dataset consist of 205 observations and 7 variables:

**Variable**|**Description**
-|-
time|Survival time in days since the operation, possibly censored.
status|The patients status at the end of the study. 1 indicates that they had died from melanoma, 2 indicates that they were still alive and 3 indicates that they had died from causes unrelated to their melanoma.
sex|The patients sex: 1=male, 0=female.
age|Age in years at the time of the operation.
year|Year of operation.
thickness|Tumour thickness in mm.
ulcer|Indicator of ulceration: 1=present, 0=absent.
stage|*additional variable based on the thickness of the ulceration (restrictions are based on research). <br> - Stage 1: thickness &le; 1 <br> - Stage 2: thickness &le; 2 <br> - Stage 3: thickness &ge; 2+

**Status**|**Summary Percentage**
-|-
Alive|65.37%
Dead|27.84%
Unrelated|6.80%

**Sex**|**Summary Percentage**
-|-
Male|62.30%
Female|37.70%

**Malignant Melanoma** is the most serious form of skin cancer - it develops from unrepairable DNA damage to skin cells, mainly caused by intense or occasional exposure to ultraviolet (UV) radiation from the sun or tanning beds, mutating skin cells to rapidly multiple and forming malignant tumors. Melanoma are most common in the form of black or brown moles (but can form in tissues as well).

The skin consists of 3 layers:
- Epidermis – outermost layer
- Dermis – second layer
- Hypodermis – last layer

When melanoma is found in the epidermis it is seen as situ or noninvasive, if found in the dermis it is seen as invasive.

Below is a table showing the stages, descriptions and survival rates for 5 years and 10 years.
<img src="images/melanoma survival chart.png"/>


<img src="images/melanoma boxplot.png"/>

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
    - **Note:** Larger thicknesses shows a higher probability in the formation of an ulceration
