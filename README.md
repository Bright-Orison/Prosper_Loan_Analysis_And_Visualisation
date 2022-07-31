# **Prosper Loan Analysis and Visualization**

## **How Borrowers characteristics influence rates charged on their loans**

**Investigation Overview**

In this analysis, I intend to look at how characteristics of borrowers could be used to predict the appropriate rate to be charged to them. I also wanted to know which categories of borrowers have the highest default risk and compare it with the categories that actually default the most.

**Dataset Overview**

The dataset used for the analysis originally contained 113,937 rows with 81 columns (depicting different variables related to each loan processed). However, for the sake of this analysis, only 21 relevant features were selected with 97752 data points maintained. The 16185 data points were deleted due to inconsistencies and missing information.
- The datasect be be accessed through the Udacity Workspace [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1581581520570000)

- Explanations on each of the variables represented by the columns can be founded in the Data dictionary [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0/ "Data Dictionary")

- After cleaning the data, 21 columns and 97752 rows were maintained in the dataset for the purpose of this analysis. The majority of the columns are numerical, but we also include date/time variables and category categories (both nominal and ordinal).

The codes below were used to import and slice the data for the relevant columns needed for the analysis👇
![image](https://user-images.githubusercontent.com/77166162/182037254-5d7f3ccf-c244-4585-a9ae-f591856d5430.png)

## **Summary of Findings**

During the exploration, I found out that there was a significant positive correlation between LenderYield and BorrowerAPR, LenderYield and BorrowerRate. This explains the fact that the lender tends to get more returns when Borrower's Annual Percentage Rate and Borrower's Rate increases.

A positive link exists between Prosper Score and Prosper Rating. There is also a strong positive correlation between Loan Status and LoanCurrentDaysDelinquent

The existence of people with relatively high salaries to their debt significantly skewed the distribution of the DebtToIncomeRatio. This is expected in a real-world scenario and does not require data changes to be applied

- Interestingly, I noticed that Unemployed people pay higher interest rates than employed people. This is because they tend to have higher risk score than the employed.

- The interest rate is inversely correlated with income.

- Also, the higher the loan amount, the lesser the rate of interest charged on it

## **Key Insights for Presentation**

For the presentation, my focus was on mainly on the main variables of interest which are Borrowers APR, Borrowers Interest Rates and how they are impacted by other variables. I started by finding the distribution of my main variables after which I introduced the other variables. 
![image](https://user-images.githubusercontent.com/77166162/182037464-627098f1-e3c5-4bf6-8f87-5783231a5246.png)
I analysed the impacts by plotting the variables using scatterplots, violin plots, boxplots, and heatmaps.
- I realised from the presentation that though, unemployed borrowers were deemed to have higher risks which translated into their payment of higher rates, the self employed borrowers rather tend to be the largest group of defaulters

After analysing the number of defaulters, it was interesting to note that full time employees defaulted the most and the non-employed borrowers were the least defaulters.
A further dive revealed that most of the full time borrowers opted for 12 months tenure wi=hich might have been the cause of the default

![image](https://user-images.githubusercontent.com/77166162/182039596-2b3f315b-a1a9-47bb-91fd-7ee3543cee3b.png)

