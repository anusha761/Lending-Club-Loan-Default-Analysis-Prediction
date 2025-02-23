# Lending-Club-Loan-Default-Analysis-Prediction
> This project focuses on analyzing loan applications from Lending Club to identify factors contributing to loan defaults. By examining applicant profiles, it aims to uncover patterns that indicate default risk, helping to mitigate credit loss. The analysis addresses the challenge of significant financial losses due to defaults, particularly among 'charged-off' customers. The objectives include pinpointing key variables that signal default risk, developing actionable insights for better risk assessment and building a machine learning model to predict defaults. Ultimately, this work seeks to enhance the Lending Club's ability to identify high-risk applicants, improve overall lending strategies and predict loan charge-off.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)



## General Information
- This project involves an exploratory data analysis of Lending Club's loan applications to identify factors influencing loan defaults, and building a machine learning model to predict defaults. By analyzing applicant profiles and historical default patterns, the project aims to enhance risk assessment, reduce credit loss for the lending institution and predict defaulter cases.
- The background of this project involves understanding the lending landscape and the financial risks associated with loan defaults. Lending Club, as a consumer finance company, faces challenges in approving loans while managing the potential for credit loss from high-risk applicants. This analysis seeks to leverage data-driven insights to inform better lending decisions and improve the overall risk management strategy.
- The business objective is to identify key driving factors behind loan defaults, understand variables that strongly indicate default risk and develop insights to improve portfolio and risk assessment and build model for predicting defaulter cases. Ultimately, the goal is to enhance Lending Club's decision-making process, leading to reduced credit loss and improved lending practices.
- The Lending Club dataset is used containing information about past loan applicants and whether they defaulted or not.



## Conclusions
1. Higher charged off cases are observed for very high loan amounts. To reduce defaulter cases, the loan amounts are recommended to stay within 17K. Also, not all loans are funded by investors.

2. High interest rates on loans is also a driving factor leading to high charge off cases. To curb down defaulter cases, a reasonable interest rate roughly within 5.4% to 11% is recommended.

3. Charged Off applicants have slightly higher Debt to Income Ratio significantly higher Revolving Line Utilization indicating they rely too much on loans and consequently cannot pay the debts. Borrowers whose Debt Income Ratio cross 15 and Revolving Line Utilization cross 45 are risky and need to be treated with caution.

4. a) As loan grade increases, from A to G, the charge off rate also increases and the grades are influenced by interest rates. Applicants in small business are taking higher graded higher interest loans, making more inquiries in last 6 months requesting for more credits, struggling with credit repay than debt consolidation and consequently getting charged off more than other purpose categories (about 26%). Lower grade loans preferably grade A should be prioritised.

 b) While rejecting people taking loans for small business purpose as they had high charge off rates, it should be ensured that no opportunity is missed while rejecting a capable applicant with small business purpose from providing loan by taking care of the nuances. Criteria for applicants taking loans for small business purpose who should not be rejected from taking loans:

  - Credit score > 0.85
  - Revolving Line Utilization rate < 35
  - Annual Income group = VH (16000.00 to 35000.00)



5. Applicants with lower income charge off more.

6. Most applicants opt for short term (36 months) loans. Applicants with long term loans (60 months) were observed to have charged off more.

7. Charged Off borrowers have lower credit score than fully paid ones. Credit score below 0.8 should be treated with caution.

8. Borrowers whose employee titles are unknown have charged off more. So it is imperative to take information about the work title of the borrowers before providing loans.



9. Weak indicators:
Although weak indicators, following patterns are observed:

  a. Applicants with higher bankruptcy records have charged off more.

  b. Charged Off applicants have paid higher late fees than fully paid ones.



Selected Model

- XGBoost : {'max_depth': 2, 'min_child_weight': 10, 'reg_alpha': 50}

- Train Accuracy: 0.9621852823952561
- Test Accuracy: 0.9569725246241576

Train Metrics

- Accuracy: 0.9621852823952561
- Precision: 0.8660
- Recall (Sensitivity): 0.8784
- F1 Score: 0.8721656260269471
- Specificity: 0.9766
- AUC: 0.9849


Test Metrics

- Accuracy: 0.9569725246241576
- Precision: 0.8428
- Recall (Sensitivity): 0.8566
- F1 Score: 0.8496376811594204
- Specificity: 0.9736
- AUC: 0.9798


## Technologies Used
- pandas - version 2.2.2
- numpy - version 1.26.4
- matplotlib - version 3.7.1
- seaborn - version 0.13.2
- scikit-learn - version 1.3.1
- scipy - version 1.13.1
- XGBoost - version 2.1.4



  ## Contact
  Anusha Chaudhuri [anusha761]
