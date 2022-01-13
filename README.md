# drug-discovery-project


* **Data** - Raw data is taken from https://www.kaggle.com/pragyanbo/a-hitchhiker-s-guide-to-lending-club-loan-data#Understanding-the-data <br/>
https://drive.google.com/file/d/1xaF743cmUgI5kc76I86AeZDE84SMkMnt/view

The dataset consists of details for more than 460,000 loans issued by the a US peer-to-peer lending company, Lending Club.

* **Tools** - The tools used were pandas, seaborn, scikit-learn.

* **Models** - To calculate the expected loss for a borrower, I used the that fact that *EL = PD x LGD x EAD*, where PD is probability of default, LGD is loss given default and EAD is exposure at default. PD was modelled using a logistic regression and EAD was modelled using a linear regression. LGD was modelled in two stages: stage 1 was used to predict if the recovery rate is 0 or not using a logistic regression and stage 2 was used to estimate the recovery rates for borrowers with recovery rate above 0 using linear regression. While calculating PD, a credit scorecard was also developed.


*Most of the information about credit risk modelling theory that I studied to build this specialized model was gained from Nikolay Georgiev's videos about credit risk modelling.
