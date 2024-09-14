Medicare Part D Claims Analysis

Overview:

I will use the Medicare Part D Claims to analyze historical healthcare expenditures. The dataset contains extensive information about healthcare providers, including their National Provider Identifier (NPI), names, credentials, gender, entity type, address, location, and rural-urban commuting area classification. The dataset has 1,287,454 records and 85 attributes. The 8 attributes of interest are “Prscrbr_Ent_Cd”, “Tot_Clms”, “Tot_Drug_Cst”, “Prscrbr_type”, “Opioid_Tot_Clms”, “Opioid_Tot_Drug_Cst”, “Opioid_Tot_Benes”, and “Opioid_LA_Tot_Clms”. In addition to the mentioned attributes, there are many more attributes available for analysis, making it a rich source of data for exploring healthcare trends and patterns. We will be utilizing Databricks for analysis to ensure efficient processing and it is a powerful data analytics platform. It stands out as the ideal tool for our project due to its robust capabilities in handling large-scale datasets such as this one. The methodology involves data collection, data cleaning, and exploratory data analysis (EDA). 
My EDA will start with an examination of prescribers' distribution across different provider types to understand the landscape of healthcare professionals contributing to prescription practices. Subsequently, I will explore prescription patterns across diverse medical specialties, focusing particularly on the top 10 specialty groups, to glean insights into workload variations and prescribing behaviors. Building upon this, I will assess the overall impact of opioid prescriptions on Medicare Part D spending and investigate the prevalence of opioid claims among beneficiaries. Finally, my analysis will scrutinize the prescribing patterns of long-acting opioids across medical specialties, elucidating the role of the top 10 specialty types in managing chronic pain. Through this analysis, I aim to illuminate the intricate interplay between provider types, medical specialties, prescription practices, and their broader implications on healthcare delivery and expenditure within the Medicare Part D program.
 
 
Data Dictionary:
1.	Prscrbr_Ent_Cd: This variable defines the type of entities reported in the National Plan and Provider Enumeration System (NPPES), which is a database used in the United States for registering healthcare providers and assigning unique identification numbers to them.
a.	"An entity code of 'I' identifies referring providers registered as individuals"
b.	"A Prscrbr_Ent_Cd of ‘O’ identifies referring providers registered as organizations"
2.	Tot_Clms: Number of Medicare D claims. 
3.	Tot_Drug_Cst: The aggregate drug cost paid for all associated claims. It encompasses all expenses related to prescription drugs covered by Medicare Part D, including ingredient costs, dispensing fees, taxes, and any applicable administration fees, and how these costs are covered by various payment sources.
4.	Prscrbr_type: variable that categorizes healthcare providers based on their specialty codes reported in Medicare claims data.
5.	Opioid_Tot_Clms: Total claims of opioid drugs, including refills.
6.	Opioid_Tot_Drug_Cst: Aggregate cost paid for opioid drugs.
7.	Opioid_Tot_Benes: The total number of unique Medicare Part D beneficiaries with at least one opioid claim.
8.	Opioid_LA_Tot_Clms: Total claims of opioid drugs, including refills.


Questions that I have answered through this analysis:

Q1) What is the distribution of prescribers by provider type?

Q2) What are the prescription patterns across various medical specialties, and what do they reveal about the workload and prescribing behavior of the top 10 specialty groups?

Q3) What is the overall impact of opioid prescriptions on Medicare Part D spending, and how prevalent are opioid claims among the beneficiary population?

Q4) How do prescribing patterns of long-acting opioids vary across different medical specialties, and what does this indicate about the role of the top 10 specialty types in chronic pain management?
