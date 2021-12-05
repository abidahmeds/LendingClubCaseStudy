# Lending Club Case Study.
> This project is about EDA Analysis on Lending Club data for past few years , covering data about their credit loan taken and other financial background about each member of the club.
Exploratory Analysis would ensure we get understanding the past behavior , the patterns , the financial evaluation score and ratios to take better decision on the new loans being offered. 


## Table of Contents
* Problem Statement and Analysis approach
* Factors for Risk Analysis of Credit Lending
* Important Univariate and Multivariate Analysis
* Final Summary
* Referenecs


## Problem Statement and Analysis Approach
> To Analyze the Lending club data set with all the information on loan given last few years and understand how some variable impacts or not towards loan success to have a loan decision made for new loans . It is important to understand the parameters which should be considered in taking loan approval decision and if some actions can be taken to secure loan customer.
### Analysis approach
- Understand credit funding parameters and factors affecting same through public knowledge and apply same on data set.
- Use EDA principles to analyse the data set 
- Clean , remove, rename and derive parameters ( columns )
- Use Data visualization methods to understand univariate and Bi variate patterns 
- Describe inferences for parameters impacting credit funding decision.


## Factors for Risk Analysis of Credit Lending
- 5 C of Credit – Character , Capacity, Collateral , Capital , Conditions 
- Credit score factors : Payment history-35% , Amounts owned -30%  , Credit history length (15%) , Credit mix(10%), New credits opened (10%).
- Credit utilization ratio = total revolving credit being used/  total of all revolving credit limits. Using more than 30% of your available credit is not good.
- Credit mix : car loan  student loan , credit card, mortgage and other credit prods , diversified mix and handling helps credit score.
- The longer the credit history , the higher the credit score.
- Number of hard enquiries lenders make towards borrower. Too much requests made in short time

## Important Univariate and Multivariate Analysis
### For detail analysis report , please refer to the Slide lendingClubCaseStudy.pdf in the attached directories.

> The following factors were considered for Analysis and also some derivative metrices were used to arrive at the analysis.
![Lending Decision Factors](https://github.com/abidahmeds/LendingClubCaseStudy/blob/master/charts/factors1.png)
![Lending Decision Factors2](https://github.com/abidahmeds/LendingClubCaseStudy/blob/master/charts/factors2.png)

### Business Driven Derived Metrices and other varaibles.
> For the purpose of Credit risk analysis , Credit Score or FICO score is to be calculated and also some other varaibles were derived out of given data columns.
- Since there is no Credit score given in Dataset , it would probably be a biz driven derived metric. 
- Payment history ( 35% of score ) = fx  { chargeoff_within_12_mths,delinq_2yrs, pub_rec , pub_rec_bankruptcies }
- Amounts owed ( 30% of Score) =  fx{ dti , revol_util , revol_bal (credit_utilization_ratio) ,   }
- Credit History Length (15% of Score) = fx{ earliest_cr_line , loandurationmonths }
- Credit Mix ( 10% Score ) = fx{opencreditlines}
- New Credits Opened (10% Score) = fx{inq_last_6mths }
> This is how Credit Score was calculated  there could be more parameters used but this is 1st version based on information gathered.
![Credit Score Calculation formula](https://github.com/abidahmeds/LendingClubCaseStudy/blob/master/charts/CreditScoreCalculationFormula.png)



## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
