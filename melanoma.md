## Malignant Melanoma Exploratory Data Analysis in R via Jupyter Notebook
Written By: Heidi

Here we will explore the [Melanoma](https://stat.ethz.ch/R-manual/R-devel/library/boot/html/melanoma.html) dataset through exploratory data analysis (EDA).

**Time Frame Conducted:** 1962 - 1977 <br>
**Location:** Department of Plastic Surgery, University Hospital of Odense, Denmark <br>
**Research Question:** Does thickness and/or ulcerated tumors have an increase chance of death from malignant melanoma?

**Synopsis of Study:** Measurements were made on patients with malignant melanoma with each patient's tumor removed. During the surgery the tumor is removed with around 2.5cm of the surrounding skin. Measurements of thickness and ulcerated presence were taken as these variables were predicted to increase the chance of death from the disease. Patients were followed until the end of 1977.

This dataset consist of 205 observations and 7 variables:

**VARIABLE**|**DESCRIPTION**
-|-
time|Survival time in days since the operation, possibly censored.
status|The patients status at the end of the study. 1 indicates that they had died from melanoma, 2 indicates that they were still alive and 3 indicates that they had died from causes unrelated to their melanoma.
sex|The patients sex; 1=male, 0=female.
age|Age in years at the time of the operation.
year|Year of operation.
thickness|Tumour thickness in mm.
ulcer|Indicator of ulceration; 1=present, 0=absent.

**Malignant Melanoma** is the most serious form of skin cancer - it develops from unrepairable DNA damage to skin cells, mainly caused by intense or occasional exposure to ultraviolet (UV) radiation from the sun or tanning beds, mutating skin cells to rapidly multiple and forming malignant tumors. Melanoma are most common in the form of black or brown moles (but can form in tissues as well).

The skin consists of 3 layers:
- Epidermis – outermost layer
- Dermis – second layer
- Hypodermis – last layer

When melanoma is found in the epidermis it is seen as situ or noninvasive, if found in the dermis it is seen as invasive.

Below is a table showing the stages, descriptions and survival rates for 5 years and 10 years.
<img src="images/melanoma survival chart.png"/>
