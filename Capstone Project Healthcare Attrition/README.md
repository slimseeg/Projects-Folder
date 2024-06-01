![Medical Match company logo](MedicalMatch.svg)

### Problem Statement

**Business Context**:

RN turnover costs a hospital 56k per nurse. The avgerage annual cost of RN turnover is 4.8M per hospital. For every 20 travel RNs eliminated, the avg hospital can save $2M.

MedicalMatch is a medtech startup committed to revolutionizing healthcare staffing. As data scientist on their product solutions team, I am tasked with analyzing healthcare employee attrition data to quantify its financial impact on hospitals and clinics. This analysis will enable the marketing team to craft targeted campaigns promoting MedicalMatch’s innovative staffing solutions.


---


### Data Dictionary:

|Feature|Type|Description|
|---|---|---|
|**age**|*int64*|Age of employee. 1: >30, 2: 30-34, 3: 35-39, 4: 40-44, 5: 45-49, 6: 50-54, 7: 55-59, 8: 60-64, 9: 65|
|**attrition**|*int64*|Did the employee leave the hospital 0: No, 1: Yes|
|**distancefromhome**|*int64*|Distance from home in miles|
|**education**|*int64*|1: High School/GED, 2: Trade/Associate, 3: Bachelor, 4: Master, 5: Doctorate|
|**environementalsatisfaction**|*int64*|1: Low, 2: Medium, 3: High, 4: Very High|
|**gender**|*int64*|Female: 0, Male: 1|
|**hourlyrate**|*float64*|Hourly pay per US BLS May 2024|
|**jobinvolvement**|*int64*|1: Low, 2: Medium, 3: High, 4: Very High|
|**jobrole**|*object*|Current job title|
|**jobsatisfaction**|*int64*|1: Low, 2: Medium, 3: High, 4: Very High|
|**maritalstatus**|*object*|Single, Married, Divorced|
|**monthlyincome**|*float64*|Monthly pay per US BLS May 2024|
|**numcompaniesworked**|*int64*|Number of previous jobs|
|**overtime**|*int64*|Did employee work overtime: No: 0, Yes: 1|
|**percentsalaryhike**|*int64*|Percent of raise|
|**performancerating**|*int64*|1: Poor, 2: Good, 3: Excellent, 4: Outstanding|
|**relationshipsatisfaction**|*int64*|1: Low, 2: Medium, 3: High, 4: Very High|
|**shift**|*int64*|Current shift. 1: 12 hr day, 2: 12 hr night, 3: 8 hr day, 4: 8 hr evening|
|**totalworkingyears**|*int64*|How many years employee has worked|
|**trainingtimeslastyear**|*int64*|How many training events employee had last year|
|**worklifebalance**|*int64*|1: Poor, 2: Moderate, 3: Good, 4: Excellent|
|**yearsatcompany**|*int64*|Total years at current company|
|**yearsincurrentrole**|*int64*|Total years in current role|
|**yearssincelastpromotion**|*int64*|Length of time in years since last promotion|
|**yearswithcurrmanager**|*int64*|How long employee has been with the same manager|




**Project Datasets**

Synthetic data taken from:

https://excelbianalytics.com/wp/downloads-21-sample-csv-files-data-sets-for-testing-till-5-million-records-hr-analytics-for-attrition/ and modified to be applicable to hospital attrition

final-healthcare.csv

**Additional Resources**

https://www.uschamber.com/workforce/nursing-workforce-data-center-a-national-nursing-crisis

https://www.nsinursingsolutions.com/Documents/Library/NSI_National_Health_Care_Retention_Report.pdf

Bureau of Labor Statistics: https://www.bls.gov/

National Library of Medicine: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2761533/

Relias: https://www.relias.com/blog/cna-turnover-costs-for-skilled-nursing-facilities#:~:text=To%20replace%20a%20CNA%2C%20an,Post%2DAcute%20Care%20at%20Relias.

---

### Executive Summary

Turnover rates in healthcare ranges from 22%+ for nurses to 55%-100% for CNAs. The average cost to replace one doctor is estimated at 500k to 1 Million. The cost to replace one nurse is estimated at 56k and the cost to replace 1 CNA ranges from 4.6K to 16K. 

MedicalMatch is a medtech staffing platform that addresses the biggest cause of healthcare attrition, burnout. One of the top causes of burnout is the lack of control over shifts. Patient and shift overload is burning healthcare staff out and contributing to turnover. MedicalMatch is the solution.

### Conclusion and Recommendations

**Age Based Attrition Observations and Recommendations**

- 33% of hospital staff are 55 and older.
   - That age bracket acounts for about half of all attrition values. 
   - With rising US RN shortages, as these employees retire, it will increase the inequality of the nurse to patient ratio.
   - Currently, the nurse to patient ratio in the US is 9 nurses for every 1,000 people.
- The cost of each RN turnover is $56,277 (NSI National Health Care Retention Report). This will be an enormous financial burden on hospitals and clinics needing to replace attrited employees.


**Recommendations:**
- Retirement is unavoidable, so emphasis needs to be placed on retention of the younger staff. Work life balance levels have an impact on attrition rates, so my recommendations are these:
   - Schedule flexibility has been cited in numerous studies (https://www.hhs.gov/surgeongeneral/priorities/health-worker-burnout/index.html) as a key factor to healthcare attrition.
   - MedicalMatch is in a strategic position to promote its platform as a solution to the need for flexible scheduling that will benefit both the hospitals, clinics and staff.

---

**Gender Attrition Observations and Recommendation**

- While men make up a third of this dataset, overall, they are about 7.5% more likely to quit.

**Recommendations:**
- This area could really use a deeper dive if more detailed data can be aquired.

---

**Job Role Attrition Observations and Recommendations**

CNA's have a 40% turnover rate, the highest of any position. 
- Per The National Institutes of Health CNA turnover rates range from 55%-100. 
- Adjusted for inflation, the cost to replace 1 CNA ranges from 4.6k-16K, plus an additional 3-6K in indirect costs.


Burnout is a common cause of healthcare attrition regardless of position. 

- CNA's have the highest patient to caregiver ratio 10/15-to-1. Patient overload can lead to "moral injury" and emotional exhaustion. (relias.com)
  - Moral Injury is a term used in healthcare to describe the guilt provider's feel for not providing the level of care they know the patient needs.

**Recommendations:**

MedicalMatch can save hospitals, clinics and especially nursing homes CNA turnover costs and should consider marketing efforts related to CNA retention.

Per the National Library of Medicine, CNA turnover in nursing homes range from 55%-100%. Further, CNAs are the "most common type of caregiver in nursing homes." This makes them a prime customer base.

---

### Model Selection and Recommendation

All of the models had similar training and testing values, which indicates that we don't have a lot of overfitting. The best model, taking into consideration overall scoring performance, was the first Neural Network model with Relu and Sigmoid Activation functions, dropout and Adam optimizer. 

Model Scores:
- Test Accuracy: 82%
- Test Recall: 82%
- Test Precision 74%
- Test F1 Score 74%
