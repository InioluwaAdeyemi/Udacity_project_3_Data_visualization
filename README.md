# Prosper Loan Data Exploration

## by Adeyemi Inioluwa


## Dataset

> The dataset contains a peer to peer loan information consisting of approximately 113,937 loans with 81 variables on each loan. The features include;  loan original amount, borrowers annual percentage rate (APR), borrower stated monthly income, loan origination date, home ownership, employment status, income range, debt to income ratio etc. You can find the dataset [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) and details about each feature [here](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&source=editors&ust=1666207824399543&usg=AOvVaw2f-n4aISScc1zmzpWtnMxv)


### Data Wrangling

> A subset of the dataframe was created with 23 columns, the data set was assessed for quality and tidiness issues. 
Columns with null values where dropped, Variables types that needed to be converted where converted to categorical types and date time.
Stated monthly income was rounded up to 2 decimal places, and True and False were replace with homeowner and not homeowner in the home ownership colum. The dataframe was transformed from 113937 entries to 77543 entries


## Summary of Findings

> In this exploration, I discovered the the Original loan amount and the Borrower's annual percentage rate(APR), have a negative relationship, hence the lower the borrower's APR, the higher the borrower's loan amount. I also discovered thet borrowers with high monthly income, guarantees a large loan amount and this was possible to depict, because of the plot matrix that showed a positive correlation between both variables

> On further investigation, I observed a strong positive relationship between, the monthly payment and loan original amount, and this made sense because monthly payments are probably calculated based on how large the loan amount is. 
Borrowers with large monthly income can get loans of huge amount. Borrowers with best prosper ratings have the lowest APR. Also, the relationship between borrower APR and loan original amount moves from negative to slightly positive when the Prosper ratings are increased from HR to A. This is probably because people with A or AA ratings tend to borrow more money, increasing APR could prevent them from borrowing more thereby maximizing the profit. But people with lower ratings tend to borrow less money, and decreasing APR could encourage them to borrow more 

> It was also oserved that Borrowers that are employed, full-time employees and self-employed, who earn high monthly incme will definitely get access to large loan amounts and  prosper ratings have a strong effect on the borrower's APR, those with the best ratings can also get access to large loan amounts.
Finally to get a large loan amount you have to have an occupation that pays a large monthly income and atleast own a house. Then a good prosper risk score of 10/11 can guarantee access to large loan amounts.

## Key Insights for Presentation

> For the presentation, I focused on the relationship between Loan Original amount and Borrower's APR, and the features that could affect them, which are borrower's monthly income(Stated Monthly Income), Prosper ratings, prosper score, monthly payment and loan term. I started out by showing the distributions of the main features, then I plotted a heat map and a matrix of scatter plots to show correlations between some of the numeric featues and the main features. 
The plots showed that Loan Original Amount and Brrower APR are negatively correlated and a very strong positive correlation between borrowers monthly income and loan amount, proving borrowers with higher monthly income can get access to more loan amounts.

> I went futher by plotting multivariate plots showing the effects of some of the features on the Loan original amount and the Borrowers APR. In the multivariate section, a plot was created to show the effect of loan term and prosper scores on the features. 
The plots showed loan term had no effect on the relationship between the main features, and Borrowers with prosper ratings of HR-C have lower APR and loan terms of 36 and 60 months, while those with ratings of B-AA have an increase in APR, with an increase in loan term.