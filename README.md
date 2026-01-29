# Data-Mini-1
Welcome to Data Mini #1! You and your teammates will have 2 hours to explore and prepare a presentation about your data analysis. The hour after will be spent presenting your findings.

This Git repository contains this `README` file and the dataset in both `CSV` and `RDS` formats. This  `README` will include the dataset's dictionary, along with the rubric and policies. The `CSV` and the `RDS` have the same rows and columns, but the `RDS` will preserve R data types exactly (factors, dates, lists, etc.). We recommend you use Duke's Container Manager to access your preferred IDE. 

## How to Participate

1. Clone this repository
2. Load the data from `data/texasdata.csv` or `data/texasdata.rds`
3. Analyze the dataset and prepare a presentation of your findings
4. Submit your presentation slides/media to ctn16@duke.edu by Monday, February 9th at 11:59pm
Please do not attempt to push changes to this repository - it is read-only for participants.

## Data Dictionary
### Student-Teacher Race Match Dataset
#### About

Same-race teachers improve academic outcomes for minoritized students, yet most never encounter a teacher who shares their racial background. Existing research highlights the benefits of race-matched instruction but often focuses on aggregate workforce diversity, obscuring students’ structural opportunities for contact. QSIDE and students at Williams College introduce race-match sufficiency—the probability that a student has at least one same-race teacher—and estimate it using administrative data from 8,691 Texas public schools serving 5.4 million students in 2022-23.

`texasdata.rds` draws on three datasets, all accessed through TEA’s Texas Academic Performance Reports (TAPR) data portal (Texas Education Agency, 2023). The Campus Reference File (CREF) provides unique campus identifiers, structural characteristics, and campus type designations; its campus–district nesting reflects the governance structure that motivates our multilevel modeling approach. The Campus Profile File (CAMPPROF) reports student and teacher demographic counts by race and ethnicity, along with total enrollment and economic disadvantage measures. Finally, district classifications come from TEA’s District type, 2022–23 release, which applies National Center for Education Statistics (NCES) geographic categories (Texas Education Agency, 2024c). Merging these files yields a raw dataset of 9,044 campuses serving nearly 5.5 million students across 1,209 districts—a census of Texas public K–12 schools.

#### Data Variables
Data

`texasdata.rds`: Cleaned campus-level dataset derived from Texas Education Agency (TEA) TAPR data and NCES district classifications. Includes:
* Student and teacher race counts
* School-level demographics and grade spans
* Charter status and district type
* Economic disadvantage proportions

| variable | mode | description |
|----------|------|-------------|
| campusName | character | |
| campusNumber | character | |
| countyName | character | |
| countyNumber | character | |
| districtName | character | |
| districtNumber | character | |
| region | factor | |
| schoolLevel | factor | |
| grade_lo | numeric | |
| grade_hi | numeric | |
| charterSchool | logical | |
| locationType | factor | |
| studentsTotal | numeric | |
| teachersTotal | numeric | |
| s_econ_disadv_prop | numeric | |
| race | factor | |
| student_frac | numeric | |
| teacher_frac | numeric | |
| student_count | numeric | |

#### Citations

This dataset was complied by Anchal Bhaskar, Kayla Chang, Iman Najib, Olivia Thornton, Jules Tucher, Régan Schwartz, and Chad M. Topaz at Williams College.

This data is freely accessible through the Institute for the Quantitative Study of Inclusion, Diversity, and Equity (QSIDE).

The citation for the replication package is:

Bhaskar, A., Chang, K., Najib, I., Thornton, O., Tucher, J., Schwartz, R., & Topaz, C. M. (2025). *Sufficiency in Teacher–Student Race Matching*. Manuscript

