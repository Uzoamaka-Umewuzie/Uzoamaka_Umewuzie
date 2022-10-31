# Loan Data Exploration
## by Uzoamaka Umewuzie


## Dataset

> The dataset contains 113,937 loan records with 81 variables (including LoanOriginalAmount, BorrowerAPR, StatedMonthlyIncome, Term, ProsperRating (Alpha), IsBorrowerHomeowner, EmploymentStatus and many others). It also contains unique identifiers/primary keys which are found under the ListingKey and ListingNumber variables. The dataset can be found [here](https://docs.google.com/document/d/e/2PACX-1vQmkX4iOT6Rcrin42vslquX2_wQCjIa_hbwD0xmxrERPSOJYDtpNc_3wwK_p9_KpOsfA6QVyEHdxxq7/pub), with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)



> Data wrangling steps include:
> 1. Changing datatypes for ListingCreationDate and ListingCategory to datetime and strings, respectively.
> 2. Changing the column name of ListingCatergory variable and replacing its numeric values with their respective categories as indicated in the data dictionary.


## Summary of Findings

> In the exploration, I found that the interest rate(BorrowerRate) is negatively correlates with original loan amount. At different size of the loan amount, the interest rate has a large range, but the range of the interest rate decreases with increase in loan amount. Borrowers with the the best Prosper ratings have the lowest inteerest rates. It means that the Interest rates strongly influences Prosper ratings.

> Borrowing pattern of both home owners and non-homeowners look the same across different period of the year. The highest listing creation were made in the month of January. Consistent increase in listings are seen from the month of August. This increase is consistent till January, consistently drops till March and is relatively even between from April to August. But comapared to non-homeowners, home owners borrow more money. This may be for debt consolidation of house mortagages as seen in the bivariate relationship between ListingCategory and IsBorrowerHomeowner.

> Also, Homeowners are probably able to access more loan amounts with respect to the current value of the home. This is because the loaners need assurance that they will be able to get back all their money if the borrower isn't able to keep up with payment. Also, for borrowers(non-homeowners)who get high interest rate even at low loan amounts, this could be because these loans are not secured as they do not involve collateral. Secured loans usually have lower interest rates than unsecured loans because the bank has a way to recoup its money if you do not pay.

> Outside of the main variables of interest, the univariate exploration of the Listing Category showed that Debt Consolidation was selected by the largest number of borrowers(more than 60,000 by count and more than 0.5 in proportion). Bivariate explorotion showed that more than 30,000 borrowers who listed Debt Consolidation are home owners. This may mean that the loans were used to pay off house mortagages.
## Key Insights for Presentation

>For the presentation, I just focused on features that could affect the Interest rate(BorrowerRate), which are original loan amount, Prosper rating. I started by showing the distribution of Interest rate and loan amount variables. Then, I showed the relationship between interest rate vs. loan amount, as well as Rating. I also investigated the effect of being a homeowner on the loan listings across months of the year and also its influence on the relationship between interest rates and loan amount.
> Increased income range amounted to increased loan amounts. Increased loan amounts amounts to lower interest rates. Lower interest rates resulted in better ratings.
