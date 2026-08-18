# Healthcare Utilization & Cost Analysis
**Author:** Malik Millner

**Date:** August 10, 2026

## Business Questions
What patient and health-condition characteristics are associated with greater healthcare utilization and higher claim payments, and where should the organization focus its resources?

I broke this down into multiple questions based on the data:
- Which health conditions are associated with the highest average claim payments?
- Is healthcare utilization associated with higher healthcare spending?
- Are patients with multiple chronic conditions associated with higher healthcare costs?
- Which diagnoses appear most frequently in the claims data?
- Does age explain healthcare spending?
- Are patients with diabetes associated with higher total claim payments?
- Are inpatient services a more important cost driver than outpatient services?
- Where should healthcare leadership prioritize its resources?

## Who Would Ask these Questions/Who would the Analysis be for?
- Healthcare Operations Managers to understand which patients and conditions are associated with greater healthcare utilization.
- Population Health Managers to identify chronic conditions associated with higher healthcare spending and prioritize care-management programs.
- Healthcare Finance and Revenue Management Teams to understand where claim payments are concentrated and which conditions are associated with higher costs.
- Care Management Teams to identify patients with multiple chronic conditions who may require additional monitoring.
- Healthcare Executives to make decisions about resource allocation, chronic-disease programs, and cost-containment strategies.

## Dataset
**Source:** [CMS.gov Synthetic PUF](https://www.cms.gov/data-research/statistics-trends-and-reports/medicare-claims-synthetic-public-use-files/cms-2008-2010-data-entrepreneurs-synthetic-public-use-file-de-synpuf/de10-sample-19)

**Size:** Over 50K—100K+ entries per table

**Description:** Contains Patient IDs, diagnostic cods, claim data, and beneficiary data surround specific visits.

**Tables Used:** 2008-2010 Beneficiary tables, Inpatient Claims, Outpatient Claims

## Tools Used 
Google Colab — Data Cleaning, Aggregation, Analysis, Transformation, and Visualization

## Key Findings
**1. Inpatient utilization is the strongest cost-related signal.** Inpatient visits had a 0.735 correlation with total claim payments, considerably stronger than outpatient utilization or chronic-condition count.

**2. Certain chronic conditions have substantially higher average claim payments.** Chronic kidney disease had the highest average claim payment at approximately $1,386, followed by stroke/TIA and COPD.

**3. Diabetes is associated with a higher cost distribution.** The diabetes-associated records showed a considerably higher median and upper total payment than non-diabetes records.

**4. More chronic conditions are associated with greater utilization, but the relationship with cost is weaker.** Chronic-condition count correlated only 0.254 with total claim payments, suggesting that simply counting diseases isn't enough to explain all the high spending.

**5. Age isn't a useful standalone predictor of spending in this analysis.** Age had only a 0.022 correlation with total claim payments, meaning age by itself provides very little explanation for variation in costs, or at least in this dataset.

## Recommendations 
- Prioritize care-management programs for high-cost conditions, particularly Chronic Kidney Disease, Stroke/TIA, COPD, and Heart Failure.
- Identify high-utilization patients and provide additional care coordination before utilization becomes more costly.
- Focus on reducing avoidable inpatient utilization with stronger discharge planning, follow-up care, and chronic-condition management.
- Use the chronic-condition count as a risk indicator when identifying beneficiaries who may require additional care management.
- Strengthen outpatient care for high-risk patients, using routine follow-ups and chronic-disease management to help prevent escalation to inpatient care.
- Create a high cost/high utilization monitoring program that tracks claim payments, inpatient visits, outpatient visits, and chronic-conditions.
- Track these metrics over time to determine whether care-management initiatives are actually associated with reductions in utilization and claim costs.
- Avoid broad cost-cutting measures and instead focus resources on the specific populations and utilization patterns identified as the greatest cost drivers.

## Conclusion
The analysis suggests that healthcare spending in this synthetic Medicare population is more strongly associated with utilization patterns and specific chronic conditions than with age alone. Inpatient utilization showed the strongest relationship with total claim payments, while chronic kidney disease, stroke/TIA, COPD, and heart failure had the highest average claim payments among the conditions analyzed. Diabetes-associated records also showed a higher distribution of total claim payments. These findings suggest that healthcare organizations could potentially improve cost management by prioritizing high-utilization patients and targeted chronic-disease management rather than relying on broad demographic characteristics such as age.

## Files
[Healtcare_Utilization_and_Cost.ipynb](https://github.com/user-attachments/files/31197822/Healtcare_Utilization_and_Cost.ipynb)    
