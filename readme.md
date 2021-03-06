# (Prosper Loan Dataset Exploration)
## by (Ujwala K)


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

## Summary of Findings

Mainly my focus was to answer below questions:-
1)Factors responsible for loan status outcome such as completed or cancelled or past-due etc
2)Factors affecting borrower's APR(which usually includes broker fees, closing costs, rebates, and discount points)
3)Factors affecting borrower's interest rate
4)Large loan amount differentiation factors(Are there differences between loans depending on how large the original loan amount was?)

In Univariate Exploration ,i plotted several plots for distribution of BorrowerAPR, BorrowerRate , DebtToIncomeRatio , Borrower's Occupation, overall LoanStatus , LoanOriginalAmount distribution plot, Income range , ProperRating and CreditGrades and observed that:-

1)Borrower APR and interest rates both fall in between 0.05 to 0.35 mostly with peak at 0.3
2)Here most of the borrower's seems to be having low DebtToIncome ratio below 43% , with a peak at 0.2 , need to check people with loan and having DebtToIncome ratio above 0.43 which is unusual
3)It seems good to see very few applications are in hold means past due and cancelled state, current and completed applications other factors of borrowers need to be investigated and very importantly what kind of borrowers became defaulters or bank Chargedoff their loan will also need to be analyzed.
4)Now lastly after observing all plots need to check their dependence like checking relation between loan status completed and current and income range and employment status and statedmonthly income 5)Prosper score and creditgrade relation seems to be analyzed with Borrower APR and interest rate

In Bivariate Exploration , several violin plots , box plots , Facet Grids , Scatterplots and heatmap and observed following points:-

1)Not employed borrowers the interest rate and APR is high almost 3.5% or 0.35
2)For income range below 25K has APR higher as compared to other higher income range borrowers
3)Most of the borrowers in the IncomeRange dollar 100000 has loan amount from 7k to 15k aprox
4)Most of the Borrowers with LoanStatus Completed , Current and ChargeOff has debt to income ratio common 0.2 , so definitely some other factors are involved in loan status decision factor which we will investigate further.
5)This correlation plot clearly shows that LoanOriginalAmount and BorrowerAPR has negative correlation with low value which of 0.323 shows their weak negative relationship hence even for higher loan amount BorrowerAPR seems to be somewhat less or same.
6)For all the lower Loan Amounts upto 15K , Loan Status shows completed and Current.
7)Most of the Borrowers with B and C Prosper and Credit ratings has Current and Completed Loan Status
8)Employmentstatus - ‘Employment ‘ has most of the LoanAmount sanctioned as per box plot quartiles , however BorrowerRate seems almost same for all the categories of mploymentstatus .
9)And Borrowers with better rating also have higher loan amount.
10)For higher Loan Amounts , term is also high.

Finally , in the multivariate exploration, with the help of Pairgrid , heatmap and pairplot , i observed findings and in addition to the finidngs of above explorations it  answered the overall questions stated in the summary point starting.
Below are this exploration findings:-
From the heat map we can see that for lower credit ratings, and lower incomes we have higher estimated returns. However income range is not influencing the estimated returns by credit rating category.
From the plots it showed that BorrowerAPR has positive relationship with EstimatedLoss and EstimatedReturn , BorrowerAPR increases with both of them.
From above Box plots ,we can observe that ChargedOff and Defaulted Loan Statuses Borrowers have higher EstimatedLoss and EstimatedReturn percentage


## Key Insights for Presentation

For the presentation, I focus on the journey of exploring the features of interest to discover which loan features are most important for loan Status and Borrower APR and Rate decisions.

I begin with introducing the features of interest one by one, followed by how they relate to one another and eventually how they correlate with each other.
