

# Introduction and Problem Statement

"BNP Paribas (BNP) is considered one of the top 5 biggest banks in Europe, according to this ranking by assets. Although BNP has grown significantly and is considered one of the largest banks in France, it also operates in most major countries within the European Union (EU). I was hired by BNP as part of the Data Team as a Data Scientist."

Last year, our company faced a problem with customer assets. Many customers closed their accounts, and the numbers raised concerns within BNP. The management aimed to reduce the customer churn rate. The Data Team received a dataset detailing customer activity, and we were tasked with analyzing the activity of customers before they closed their accounts. 

The Data Team asked me to analyze this detailed activity dataset and derive several actionable insights from it. Furthermore, they intend to build a predictive model based on customer activity. The model should be capable of predicting customer behavior in relation to churn. For instance, the model might predict that Customer A has a high likelihood of remaining a customer. In another case, Customer B's activity may resemble that of a customer likely to close their account. Therefore, the bank could offer targeted ads or campaigns to retain this customer, or potentially turn them into a loyal customer.

The management has also requested additional insights from the dataset, with the goal of enabling further actionable, data-driven decisions. To summarize, our objectives are as follows: derive key insights from the data, build a predictive model for customer churn, and use recall as the evaluation metric to assess the model's performance. These are the primary tasks to be accomplished.

Another information to read about the importancy of customer churn rate to stay low [link1](https://static.googleusercontent.com/media/research.google.com/id//pubs/archive/36678.pdf) [link2](https://mtarget.co/blog/mengenal-customer-churn/)



# Summary 

## Model Recap 
We used six different models and found that the RF model performed better than the others. Initially, it achieved a recall score of 0.75 on testing and 0.74 on training. After applying cross-validation, the model's performance improved, with recall increasing to 0.76 on testing and 0.8 on training. The model remains a good fit, and there is an improvement in the recall score on the testing data.

## Insight 

We need further investigation into customer behavior due to indications in the data that customers with high balance groups tend to have a higher total churn rate. Germany has a higher balance compared to other countries, so it may be valuable to deepen insights into the German market by offering investment services through our bank, particularly in capital investment deposits or banking products that generate income for them. This approach could increase our profits while lowering our churn rate, as customers with more services from us are likely to stay more engaged. Similarly, active members have a lower chance of churn compared to passive members. We could focus on high balance customers, defined as those with over 100,000 Euros.

The model has shown good performance and is ready for deployment, as it is a good fit with a recall score of 76%. Although there is potential to improve the model further with boosting algorithms such as XGBoost or other boosting techniques, it would be helpful to add correlations that provide stronger determinants. Currently, only one feature shows a moderate correlation among the numerical data, and ideally, other features could support the model in capturing patterns more effectively


# URL
[Kaggle datasets](https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction/data)

[Hugging Face](https://huggingface.co/spaces/asanmaulana/churn_model_banking)



