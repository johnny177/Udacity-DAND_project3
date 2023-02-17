# ProsperLoan Dataset Exploration
## by John Ametepe Agboku 


## Dataset

> The ProsperLoan dataset contains 113,937 loans with 81 variables on each loan. 
> 14 features was selected to investigate the dataset. And they are:
>1. LoanOriginationDate
>2. Term
>3. BorrowerRate
>4. LoanOriginalAmount
>5. IncomeRange
>6. CurrentDelinquencies
>7. DelinquenciesLast7years
>8. ProsperRating (Alpha)
>9. Occupation
>10. EmploymentStatus
>11. IsBorrowerHomeowner
>12. MonthlyLoanPayment
>13. LoanStatus
>14. ProsperScore
>
> LoanOriginalAmount, CurrentDelinquencies and DelinquenciesLast7Years were selected as the features of interest, however, through the investigation, I found out the Delinquencies features have little or no relationship with the other features. So, only timeseries exploration was done.
> ProsperScore and ProsperRating (Alpha) was orginated after July 2009 according to the data dictionary so, in order not to make a bias investigation/ analysis, i dropped loans before July 2009.
And I discovered some interesting trends and relationships.
> The data downloaded from 
> And the data dictionary can be found [here] (https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)


## Summary of Findings

>From, my investigations, I found out that, the Total LoanAmount per month increased steadily over the years until the latter months of 2012 wherer there was a fall but after the fall there was surge in the 2013 and a sharp decline in the early months of 2014
> I again discovered that the more Borrowers are Homeowners and these homeowners take larger loan anount than non homeowners with the same IncomeRange as them.
> Moreover, Most of the LoanAmount is concentrated around 5000. And also, the LoanAmount with longer Term have a smaller MonthlyLoanPayment but increases as the LoanOriginalAmount increases but has a lower BorrowerRate and vice versa. Generally, as the LoanAmount increases so does the MonthlyLoanPayment but the BorrowerRate decreases.
> Again, loans with long Term have low MonthlyLoanPayment as compared to the other short Terms but have higher BorrowerRate.Therefore, the longer the Term of loan, the lower the MonthlyLoanPayment but with higher BorrowerRate and vice versa.
> Further, the loans with lower MonthlyLoanPayment have the best ProsperScore and Rating.

## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.
> I focus on how the BorrowerRate and MonthlyLoanPayment determines the LoanOriginalAmount. I left out the Delinquencies features since nothing interesting was determined about them for the presentation
> I start by looking at the timeseries of the LoanOriginalAmount and its distribution.
> And then, i look at the relationships between the three forementioned features.
> 
> To add with, I looked at the Categorical features one after the other. To start with, I use the Violin plots to look at the LoanOriginalAmount, BorrowerRate and MonthlyLoanPayment relationship with the categorical variables.
> Later, I use barplots to look at the relationship between LoanOriginalAmount, ProsperRating (Alpha), ProsperScore and IsBorrowerHomeowner
> 
> I am looking at the scatterplots of LoanOriginalAmount and MonthlyLoanPayment and BorrowerRate with the categorical variables each has a third variable where the categorical featuresa are indicated as colors with clear color differences that are easy to identify to show how these categorical features influence the LoanOriginalAmount