# Lendingclub-loan
1 Introduction LendingClub is a peer to peer lending company in which their product allows consumers to both invest and borrow loans. They offer multiple kinds of loans like student loans, personal loans, auto refinancing loans and even business loans. The borrowers who are interested in obtaining loans will get a loan grade assigned to them which affect their interest rates and the amount of money they can borrow. A lot of the LendingClub data leads to insightful conclusions about the borrowing and investing patterns of all kinds of individuals. Through our investigation, we will explain patterns and similarities of the behaviors of borrowers and investors. 1.1 Questions of Interest We intend to start off with exploratory data analysis of all the factors involved to find patterns and relationships. We will look at the data from multiple angles to get a sense of the intricacies that lie within the data. We will additionally match the trend we see in the data to external events to try to explain why such is happening. We will also conduct time series decomposition in regards to the average loan amounts being requested. We will take a look at the trend and the seasonality so that we can better forecast spikes in demand. After, we will try to fit prediction models in order to answer a couple questions: namely whether a loan request from a client should be funded or not from the perspective of the bank, and what interest rate a borrower would get for a loan from the perspective of a client. After finding good models, we will deconstruct them in order to get a deeper sense of the important aspects in such decisions. 1.2 Dataset The dataset we are using is a compilation of data on loans issued by LendingClub from the period 2007 to 2015. The data includes information on the current loan status (how much has been funded so far, how much has been paid off, etc) as well as information about the borrower (occupation, income, credit score, etc). This data lends itself to a variety of interesting financial analysis, notably time series analysis since the data is date stamped. We will touch on a number of variables present in the dataset throughout the course of this analysis. We will consolidate the meanings of all these variables here for future reference. • loan_amnt: listed amount of the loan applied for by the borrower • funded_amnt: total amount committed to that loan at that point in time • funded_amnt_inv: total amount committed by investors for that loan at that point in time • term: number of payments on the loan. Values are in months and can be either 36 or 60 • int_rate: interest rate on the loan University of California, Davis • installment: monthly payment owed by the borrower • grade: loan grade that corresponds to the risk of the loan • loan_status: current status of the loan • total_bal_il: total current balance of all installment accounts • emp_title: job title of the borrower • next_pymnt_d: next scheduled payment date • sec_app_mort_acc: number of mortgage accounts at time of application for the secondary applicant More information about the dataset can be found here: https://www.kaggle.com/wendykan/lending-club-loan-data
LendingClub is a peer to peer lending company in which their product allows consumers to both
invest and borrow loans. They offer multiple kinds of loans like student loans, personal loans, auto
refinancing loans and even business loans. The borrowers who are interested in obtaining loans will
get a loan grade assigned to them which affect their interest rates and the amount of money they
can borrow. A lot of the LendingClub data leads to insightful conclusions about the borrowing and
investing patterns of all kinds of individuals. Through our investigation, we will explain patterns and
similarities of the behaviors of borrowers and investors.
1.1 Questions of Interest
We intend to start off with exploratory data analysis of all the factors involved to find patterns and
relationships. We will look at the data from multiple angles to get a sense of the intricacies that lie
within the data. We will additionally match the trend we see in the data to external events to try to
explain why such is happening.
We will also conduct time series decomposition in regards to the average loan amounts being requested.
We will take a look at the trend and the seasonality so that we can better forecast spikes in demand.
After, we will try to fit prediction models in order to answer a couple questions: namely whether a
loan request from a client should be funded or not from the perspective of the bank, and what interest
rate a borrower would get for a loan from the perspective of a client. After finding good models, we
will deconstruct them in order to get a deeper sense of the important aspects in such decisions.
1.2 Dataset
The dataset we are using is a compilation of data on loans issued by LendingClub from the period
2007 to 2015. The data includes information on the current loan status (how much has been funded so
far, how much has been paid off, etc) as well as information about the borrower (occupation, income,
credit score, etc). This data lends itself to a variety of interesting financial analysis, notably time
series analysis since the data is date stamped.
We will touch on a number of variables present in the dataset throughout the course of this analysis.
We will consolidate the meanings of all these variables here for future reference.
• loan_amnt: listed amount of the loan applied for by the borrower
• funded_amnt: total amount committed to that loan at that point in time
• funded_amnt_inv: total amount committed by investors for that loan at that point in time
• term: number of payments on the loan. Values are in months and can be either 36 or 60
• int_rate: interest rate on the loan
University of California, Davis
• installment: monthly payment owed by the borrower
• grade: loan grade that corresponds to the risk of the loan
• loan_status: current status of the loan
• total_bal_il: total current balance of all installment accounts
• emp_title: job title of the borrower
• next_pymnt_d: next scheduled payment date
• sec_app_mort_acc: number of mortgage accounts at time of application for the secondary
applicant
More information about the dataset can be found here:
https://www.kaggle.com/wendykan/lending-club-loan-data
