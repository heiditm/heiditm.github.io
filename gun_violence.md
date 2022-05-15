## Gun Violence
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
