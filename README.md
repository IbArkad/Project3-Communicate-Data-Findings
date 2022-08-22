# The Loan Original Amount For Borrowers And Its Interactions With Some Other Loan Features.
## by: Dominic Ibamondor Bakantiche)


## Dataset: Prosper Loan

> The dataset originally contained information on 113,937 personal loans given by Prosper to borrowers with at least a credit score of 600. After cleaning out an out of range Prosper score, 11.0, the dataset for the investigation now contains 112481 borrowers information. On each loan, there are 81 variables including the loan original amount, borrower rate, stated monthly income, monthly loan payment, employment status, Prosper score, current loan status, and many others. Prosper used a proprietary rating system that considered data points like credit history and debt-to-income ratio to determine the Prosper score of a borrower, which investors relied on to decide whether to fund the loan or not. Most loans were funded within three days, and potential borrowers whose applications were not at least 70% funded expired within 14 days.

## Summary of Findings

### EDA Steps
> In exploring the Prosper loan dataset to gain insights, I set off by first investigating to understand the distribution of the feature of interest, the loan original amount, and other features including loan status, loan origination quarter, monthly loan payment, Prosper score, Is borrower homeowner, employment status, borrower state and borrower annual percentage rate (APR). At this stage, since these were univariate analysis, bar plots and histograms were used depending on whether the data of the particular feature were quantitative or qualitative. 

> The univariate analysis was followed with bivariate analysis to study the relationship between the loan original amount and the other features, and the relationship between some of the other features. Depending of the data type combination box plots, violin plots, scatter plots, faceted histograms, clustered bar charts were built. 

> Multivariate analysis was carried out to understand how at least any two of the other features interacted with the loan original amount by  faceting different plot types were used. 



### Univariate analysis

> The histogram of the the loan original amount is unimodal and right-skewed. The log tranformation of the scale is telling in the normal distribution where the median of the distribution is about 4000 on the logarithmic loan original amount scale. 

> 56576 are current loans, 38074 loans are completed, 11992 are chargedoff, and 5018 defaulted. 5 loans are cancelled and the remainder are loans which have past due dates for at least 1 day and beyond 120 days.

> In the decending order of loan origination, most loans originated in the second quarter of the year 2009 (Q2 2009) followed by those originated in Q4 2005, Q4 2008 and Q1 2006. The least count of loans originated in Q1 2014 and Q3 2007. Different counts of loans were originated in the other quarters of the years between 2006 and 2014, inclusive.  

> Base on the Prosper score and applicable to loans originated after July 2009, 992 of the loans were high risk and 4750 loans were lowest risk or best loans. These two extremes were still lower than the majority of Prosper loans given to borrowers. 

> More homeowners took loans than those who did not own a home. 57478 against 56459 borrowers owned a home.

> For the employment status of borrowers, 67322 were employed, 26355 were full-time, 6134 were self-employed. Beyond these the remainder of the borrowers were either not available, were part-time employees, not employed, retired or classified under other types of employment. 795 of the remainder of over 110000 borrowers were retired.

> Lending was not evenly distributed to borrowers from all the states. Borrowers from the state of CA were the most to apply for loans and the most likely to have their loan applications granted as compared to those of ND. 



### Bivariate analysis

> The median loan original amount for the loan status Current is the highest while the median loan original amount of the loan status Cancelled is the lowest. Loan status Completed, Current and Past Due (1-15 days) were multimodal, while majority of the other loan status were unimodal with loan original amount concentrated almost around their respective median.


> While the distribution of most of levels of the loan origination quarter in relation to the loan original amount are unimodal and right-skewed, those of Q1 2012, Q2 2012, Q3 2012, Q2 2013, Q3 2013, Q4 2013 and Q1 2014 have their modes occur at a count of at least 2000 borrowers. The Q2, Q3 and Q4 of the year 2013 had a wide spread of loan original amount and count of borrowers, as did the Q1 of the year 2014.

> There is a positive correlation between the loan original amount and the monthly loan payment. The monthly loan payment increased with increasing loan original amount.

> The relationship between the loan original amount and Prosper score is such that, the highest risk Prosper Score of 1.0 has the lowest median loan original amount, as well as one of the levels of the risk score with a lot of outliers too. The Prosper Scores 8.0 and 10.0 have about the same median loan original amounts, which are also the highest median values. The median loan original amount of all other levels of Prosper Score were withing boundaries of 1.0 and 10.0 of Prosper score, with the exception of that which was observed for the Prosper score of 8.0.

> Borrowers owning homes recorded a higher loan original amount median compared to those without homes. The first quartile, third quartile and maximum value for home owners are also greater than those without homes which also saw a lot of outliers.

> The relationship between the loan original amount and the employment status of the borrowers is such that the Employed level which has a multimodal distribution has the highest median, while the borrowers classified under the Not availabe employment status have the lowest median. The remaining status have varying median and shape of their respective distributions, most of which are unimodal.

> The borrower state does relate significantly with the loan original amount. Borrowers from the state of CA are significant to the customer base of Prosper loan. Borrowers from CA are the predominant customers of Prosper loan, and comparably also have a good number of debtors apply for very large loan original amount. It is also the state that records the most of borrowers wanting the smallest loan original amount. The distribution of the loan original amount across the states of the borrowers are largely unimodal, not normally distributed and are skewed to the right. The number of borrowers as well as the loan original amount applied for by customers from the states of ND, SD, IA, AK, ME, WY, VT, NH, HI, MT, ID, TN, NM, DE, AR, SC, NE, UT, OK, KY, DC, RI, WV, LA, NV, AL, AZ, MD, VA, PA, OR, NI, WA, OH, NC and MS are fairly insignificant compared to those of the others states. The most of the borrowers of Prosper loan who request large loan amounts are from the states of CA, GA, II, FL, NY and TX.

> There is a negative correlation between the loan original amount and the borrower annual percentage rate (APR). The borrower APR decreased with increasing loan original amount. The interaction of the loan original amount and the borrower APR overlap each other and very concentrated in the borrower APR range of about 0.07 and 0.4, and loan original amount of 0 and 25000 dollars.



### Multivariate analysis

> The loan original amount and the monthly loan payment are strongly correlated across all the states from where borrowers come, despite all the states having varying borrowers population, who also applied and received different loan amounts, and charged different monthly loan payment amounts based on the loan amount received.

> Each employment status interacted differently with Prosper score and the loan original amount. The interaction of the employment status Self-employed and Employed with the Prosper score and the loan original amount was more pronounced and strong, than was observed for the employment status Not employed, Part-time and Retired. The borrowers who were Self-employed and Employed were more and, their respective Prosper score and the loan original amount were also higher as compared to the borrowers of the other employment status types.

> With the loan original amount correlating strongly with the monthly loan payment, majority of the borrowers had an APR between 0.1 and 0.4 charged on the range of the loan original amount.

> Completed, DefaultedLoanStatus and ChargedOff were the loan status that interacted with the borrower state across the range of the loan original amount. Different levels of the loan status distributed differently across the states. While some of the distributions were unimodal, others were multimodal. The median loan original amount was different for all the loan status levels of all the borrower states.

> Regardless of the status of ownership of a home by a borrower, the monthly loan payment increased with increasing loan original amount.




## Key Insights for Presentation

> The presentation of the key insights drawn from the exploration of the Prosper Loan dataset focuses on the loan original amount, Prosper score, monthly loan payment, borrower state and the borrower annual precentage rate (APR). At the outset, I give an understanding into the distribution of the feature of interest, the loan original amount with a histogram since it is a quantitative data. I produced two histogram plots for the feature since the plot of the initial loan original amount was right-skewed. To create a normal distribution histogram of the feature, I performed a log transformation of its axis.  

> I then followed this with a box plot of the various levels of the Prosper score to understand how they each relate with the loan amount. I was also interested in understanding the relationship between the loan amount and the monthly loan payment made by each of the borrowers, and therefore created a scatter plot which was best suited to grant this.

>To know the relationship between the loan payment and loan amount as distributed across each of the 51 states, I created a facetedgrid of scatter plot, as this was important for me to know which state's borrowers took loans the most, the amounts taken and the magnitude of money repaid back to Prosper on a monthly basis. 

> Finally, a scatter plot to understand the distribution of the borrower APR charged on the loan original amount given out, and the corresponding monthly payment was created, and was telling in revealing the range of APR charged on majority of the loans. 