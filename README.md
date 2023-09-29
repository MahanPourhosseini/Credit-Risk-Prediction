### Problem Statement
Credit risk infers to the possibility of a loss emerging from a borrower's downfall to pay back a loan or meet contractual commitments. Conventionally, it pertains to the risk arising from lenders' inability to return the owed interest and principal, impacting the cash flows and increasing assemblage costs.
In this session, we used German credit data.The aim is to predict credit risk when a person requests for loan.
You have to build a model to predict whether the person, described by the attributes of this dataset, is a good (1) or a bad (0) credit risk?


### Attribute Information
Credit risk dataset contains 1000 samples and 21 attributes. A brief description for each attribute is as follows:

#### Categorical Features:

1) **status**: status of the debtor's checking account with the bank

  - 1 : no checking account
  - 2 : ... < 0 DM
  - 3 : 0<= ... < 200 DM
  - 4 : ... >= 200 DM / salary for at least 1 year

2) **credit_history**: history of compliance with previous or concurrent credit contracts

 - 0 : delay in paying off in the past
 - 1 : critical account/other credits elsewhere
 - 2 : no credits taken/all credits paid back duly
 - 3 : existing credits paid back duly till now
 - 4 : all credits at this bank paid bac

3) **purpose**: purpose for which the credit is needed

 - 0 : others
 - 1 : car (new)
 - 2 : car (used)
 - 3 : furniture/equipment
 - 4 : radio/television
 - 5 : domestic appliances
 - 6 : repairs
 - 7 : education
 - 8 : vacation
 - 9 : retraining
 - 10 : business

4) **savings**: debtor's savings

 - 1 : unknown/no savings account
 - 2 : ... <  100 DM
 - 3 : 100 <= ... <  500 DM
 - 4 : 500 <= ... < 1000 DM
 - 5 : ... >= 1000 DM

5) **personal_status**: combined information on sex and marital status

 - 1 : male : divorced/separated
 - 2 : female : non-single or male : single
 - 3 : male : married/widowed
 - 4 : female : single

6) **other_debtors**: Is there another debtor or a guarantor for the credit?

 - 1 : none
 - 2 : co-applicant
 - 3 : guarantor

7) **other_installment_plans**: installment plans from providers other than the credit-giving bank

 - 1 : bank
 - 2 : stores
 - 3 : none

8) **housing**: type of housing the debtor lives in

 - 1 : for free
 - 2 : rent
 - 3 : own

#### Binary features
9) **people_liable**: number of persons who financially depend on the debtor (i.e., are entitled to maintenance)

 - 1 : 3 or more
 - 2 : 0 to 2

10) **telephone**: Is there a telephone landline registered on the debtor's name?

 - 1 : no
 - 2 : yes (under customer name)

11) **foreign_worker**: Is the debtor a foreign worker?

 - 1 : yes
 - 2 : no

#### Ordinal features:

12) **employment_duration**: duration of debtor's employment with current employer

 - 1 : unemployed
 - 2 : < 1 yr
 - 3 : 1 <= ... < 4 yrs
 - 4 : 4 <= ... < 7 yrs
 - 5 : >= 7 yrs

13) **installment_rate**: credit installments as a percentage of debtor's disposable income

 - 1 : >= 35
 - 2 : 25 <= ... < 35
 - 3 : 20 <= ... < 25
 - 4 : < 20

14) **present_residence**: length of time (in years) the debtor lives in the present residence

 - 1 : < 1 yr
 - 2 : 1 <= ... < 4 yrs
 - 3 : 4 <= ... < 7 yrs
 - 4 : >= 7 yr

15) **property**: the debtor's most valuable property, i.e. the highest possible code is used. Code 2 is used, if codes 3
or 4 are not applicable and there is a car or any other relevant property that does not fall under variable
sparkont.

 - 1 : unknown / no property
 - 2 : car or other
 - 3 : building soc. savings agr./life insurance
 - 4 : real estate

16) **number_credits**: number of credits including the current one the debtor has (or had) at this bank

 - 1 : 1
 - 2 : 2-3
 - 3 : 4-5
 - 4 : >= 6

17) **job**: quality of debtor's job

 - 1 : unemployed/unskilled - non-resident
 - 2 : unskilled - resident
 - 3 : skilled employee/official
 - 4 : manager/self-empl./highly qualif. employee

#### Continuous features:

18) **duration**: credit duration in months

19) **amount**: credit amount in DM

20) **age**: age in years


#### Class labels:
21) **credit_risk**: Has the credit contract been complied with (good) or not (bad) ? (binary class)

 - 0 : bad
 - 1 : good


![download (1)](https://github.com/MahanPourhosseini/Credit-Risk-Prediction/assets/144378675/a05c0330-5752-43c3-8fb6-6bef2fc92956)


