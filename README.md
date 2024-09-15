# Medicare Part D Analysis 

## Overview

I will use the Medicare Part D Claims dataset to analyze historical healthcare expenditures. The dataset contains extensive information about healthcare providers, including their National Provider Identifier (NPI), names, credentials, gender, entity type, address, location, and rural-urban commuting area classification. The dataset comprises 1,287,454 records and 85 attributes. For this analysis, we will focus on the following 8 attributes:

- `Prscrbr_Ent_Cd`
- `Tot_Clms`
- `Tot_Drug_Cst`
- `Prscrbr_type`
- `Opioid_Tot_Clms`
- `Opioid_Tot_Drug_Cst`
- `Opioid_Tot_Benes`
- `Opioid_LA_Tot_Clms`

In addition to these attributes, there are many more available for analysis, making it a rich source of data for exploring healthcare trends and patterns. We will utilize Databricks for analysis to ensure efficient processing, as it is a powerful data analytics platform well-suited for handling large-scale datasets.

## Methodology

1. **Data Collection**
2. **Data Cleaning**
3. **Exploratory Data Analysis (EDA)**

### EDA Plan

1. **Examine Prescribers' Distribution**
   - Analyze the distribution of prescribers across different provider types to understand the landscape of healthcare professionals contributing to prescription practices.

2. **Explore Prescription Patterns**
   - Investigate prescription patterns across diverse medical specialties, with a focus on the top 10 specialty groups, to gain insights into workload variations and prescribing behaviors.

3. **Assess Impact of Opioid Prescriptions**
   - Evaluate the overall impact of opioid prescriptions on Medicare Part D spending and investigate the prevalence of opioid claims among beneficiaries.

4. **Analyze Long-Acting Opioid Prescribing Patterns**
   - Scrutinize prescribing patterns of long-acting opioids across medical specialties to elucidate the role of the top 10 specialty types in managing chronic pain.

## Data Dictionary

1. **Prscrbr_Ent_Cd**: Defines the type of entities reported in the National Plan and Provider Enumeration System (NPPES).
   - `'I'`: Referring providers registered as individuals.
   - `'O'`: Referring providers registered as organizations.

2. **Tot_Clms**: Number of Medicare D claims.

3. **Tot_Drug_Cst**: Aggregate drug cost paid for all associated claims, including ingredient costs, dispensing fees, taxes, and any applicable administration fees.

4. **Prscrbr_type**: Categorizes healthcare providers based on their specialty codes reported in Medicare claims data.

5. **Opioid_Tot_Clms**: Total claims of opioid drugs, including refills.

6. **Opioid_Tot_Drug_Cst**: Aggregate cost paid for opioid drugs.

7. **Opioid_Tot_Benes**: Total number of unique Medicare Part D beneficiaries with at least one opioid claim.

8. **Opioid_LA_Tot_Clms**: Total claims of long-acting opioid drugs, including refills.

## Questions Answered

1. **What is the distribution of prescribers by provider type?**

2. **What are the prescription patterns across various medical specialties, and what do they reveal about the workload and prescribing behavior of the top 10 specialty groups?**

3. **What is the overall impact of opioid prescriptions on Medicare Part D spending, and how prevalent are opioid claims among the beneficiary population?**

4. **How do prescribing patterns of long-acting opioids vary across different medical specialties, and what does this indicate about the role of the top 10 specialty types in chronic pain management?**
