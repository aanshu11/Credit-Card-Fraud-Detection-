# Credit-Card-Fraud-Detection- 

## Business Understanding 

* Finex is a leading financial service provider based out of Florida, US. It offers a wide range of products and business services to customers through different channels, ranging from in-person banking and ATMs to online banking. Over the last few years, Finex has observed that a significantly large number of unauthorized transactions are being made, due to which the bank has been facing a huge revenue and profitability crisis. 

* Many customers have been complaining about unauthorized transactions being made through their credit/debit cards. It has been reported that fraudsters use stolen/lost cards to access the personal and sensitive data of many cardholders.  Other ways in which Fraudulent transactions take place is skimming, alteration of genuine credit cards, counterfeit cards.

* In most cases, customers get to know of such unauthorized transactions happening through their cards quite late as they are unaware of such ongoing credit card frauds or they do not monitor their bank account activities closely. This has led to late complaint registration with Finex and by the time the case is flagged fraudulent, the bank incurs heavy losses and ends up paying the lost amount to the cardholders.


## Objective 

* To develop a machine learning  model to detect fraudulent transactions based on the historical transactional data of customers with a pool of merchants. 

* To recommend optimal ways and preferable machine learning model Finnex can employ to mitigate fraud risks and prevent  heavy financial losses.

* Demonstrating the potential benefits  of the final model through a cost-benefit analysis in order to analyse the business impact of fraudulent transactions. 

## Data Understanding 

The data set contains credit card transactions of around 1,000 cardholders with a pool of 800 merchants from 1 Jan 2019 to 31 Dec 2020. It contains a total of 18,52,394 transactions, out of which 9,651 are fraudulent transactions. 

The data set is highly imbalanced, with the positive class (frauds) accounting for 0.52% of the total transactions. 
Now, since the data set is highly imbalanced, it needs to be handled before model building. The feature 'amt' represents the transaction amount. The feature 'is_fraud' represents class labelling and takes the value 1 the transaction is a fraudulent transaction and 0, otherwise.

The dataset can be downloaded using this link [Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection).

![image](https://user-images.githubusercontent.com/80308356/195155865-b5791193-cfca-48de-986c-560aa2475931.png)


## Project Pipeline 

* Reading and Understanding the data - Loading the data and understanding the features present in it.
* Exploratory Data  Analysis (EDA) -  Univariate, Bivariate analysis, Feature Transformations, mitigating skewness etc . 
* Train/Test Splitting    -    Stratified k-fold cross validation 
* Model Building and Hyperparameter tuning - Starting with baseline linear model before going towards ensemble . 
* Model Evaluation - The area under the ROC curve (known as AUC ROC) is the most widely used metric to assess the performance of fraud detection systems with imbalanced Data. We have to focus on High AUC and High recall in order to detect actual fraudulent transactions.
* Business Impact - Cost Benefit analysis to demonstrate potential benefits. 

![image](https://user-images.githubusercontent.com/80308356/195155656-5e197a8f-671f-4354-a1bc-96841a6a0b7d.png)



## Cost Benefit Analysis 

* After the model has been built we perform a cost-benefit analysis to demonstrate its potential benefits. For this we compared the cost incurred before and after the model is deployed.

*  Cost incurred per month before the model was deployed = Average amount per fraudulent transaction * Average number of fraudulent transactions per month

*  cost incurred per month after the model is built and deployed = 1.5*TF + Average amount per fraudulent transaction * FN.

*  Final savings = Cost incurred before - Cost incurred after.


![image](https://user-images.githubusercontent.com/80308356/195156087-7163a202-5afd-4d25-9bc7-f7539953cbe3.png)

![image](https://user-images.githubusercontent.com/80308356/195156118-997d178a-2535-44f6-b0d8-876aa1bf1b56.png)



## Video Presentation 

Video Presentation link - [Link](https://drive.google.com/file/d/1-05B-yJk42teMP9AyZfQTLnZEPrZ8ijF/view?usp=sharing).






