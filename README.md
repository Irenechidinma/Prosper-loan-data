# Prosper Loan Dataset
# By Nwajagu Irene

Dataset
This project I have used one of the curated data sets, provided by Udacity. It is the prosper loan data set, that contains information about loan listings and related variables including borrower as well as lender information. It contains variables related to Borrower such as credit rating, prosper rating etc. The dataset also has the lender information.

During the course of this project I was able to import the necessary libraries and load the data. I accessed the dataset programatically to check for duplication and null values of which the duplicates were dropped.

Summary of Findings
The BorrowerAPR distribution looks multimodal. it showed small peak centered at 0.1, a large peak centered at 0.2. There is also a small peak centered 0.3. Additionally, there is a very sharp peak between 0.35 and 0.36. Only very few loans have APR greater than 0.43.

Borrower APR is highly correlated with Borrower Rate.If borrower rate increases borrower APR will also increase and vice-versa. There is a moderate correlation between investors and Loan original amount. It is strange that debt to income ratio is very low correlated with every other variable. It could be due to not including large number of features from main dataframe 'df'. But I will try to explore this feature with categorical variables. Also, if we look at the DTI (debt to income ratio) graph (pairplot) and compare it with the graphs of borrower APR and borrower Rate, we can observe that their is some correlation between these variables. There seem to be some outliers present in credit score range upper and credit score range lower variables. I will remove them and then again plot the pairgrid to see the correlation. There is moderate negative correlation between loan original amount and Borrower APR, Borrower Rate variables.

Out of all loan status, 'completed' and 'current' status are the only ones with maximum count of APR and rate less than or equal to 0.2.If borrower APR and rate are high then loan status is more likely to be anything except 'current' and 'completed'.

Key Insights For Presentation
For the presentation, I just focus on features that could affect the borrower APR, which are original loan amount, loan status and employment status. I started by showing the distribution of borrower APR and loan status. Then, I showed the relationship between APR vs. borrower's rate, as well as APR vs. loan status.

