# PR_Loan_Analysis
This is a project which analyzes loan data for Udacity.
# Prosper Loan Data Exploration
## by Angie Koepcke


## Dataset

> The Prosper Loan data set contains loan data for various types of loans from 2005-2014. The data file was provided by Udacity.

> The first step I completed was to upload the 'prosperLoanData.csv' file to my project folder in my jupyter notebook.  This way I could run .head() and .info() on the data and get an idea of what I was looking at.  I opened the Prosper Loan Data variable definitions in Google sheets.

> I also check to make sure all the packages I needed for this project were installed.  It turned out I had to install Seaborn, so I did this in Linux. After installing Seaborn, I checked the data using .head() and .info(). 

> There were 80 columns and 113,937 rows of data in the loan data file.  I had to decide which variables I wanted to explore.  The loan listing category, which classifies what the loan was for, and the state interested me right away.  Beyond that, I decided I needed to do more exploration and make some decisions. 

> There were rows with duplicated data, so I decided to drop the rows. I ran code to see which columns were involved in the data duplication, and dropped the rows based on the 'ListingNumber' column.

> Some of the columns weren't in an ideal format for analysis.  I changed some object columns to datetime so I could analyze data across time periods.  These columns included, 'ListingCreationDate', 'DateCreditPulled', 'ClosedDate', and 'LoanOriginationDate'.  Doing this allowed me to see that this data creation ranges were between the years 2005 to 2014.


## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

> California Texas, New York, Florida and Illinois had the most loans with Prosper. There were 112,239 unique loans listings. There were over 5,000 loans which didn't provide the data for the state.

> The loans ranged in terms from 12 to 60 months. The approximate average length of a Prosper Loan is 41 months.

>
> It appeared that the borrowers occupation being listed as 'Other' was correlated with more net losses on loans.
>


## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.
> The loans with occupation listed as 'Other' seemed to be at risk for default.
> Some states had higher rates of default than others.  There were loans where a state wasn't even present in the data.



## Sites visuted during analysis
> https://stackoverflow.com/questions/38134012/pandas-dataframe-fillna-only-some-columns-in-place
> https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.nlargest.html
> https://www.kaggle.com/xdurana/multivariate-analysis-and-correlation-matrix
> https://datatofish.com/statsmodels-linear-regression/
