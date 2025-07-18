# Churn-Prediction
PowerCo  Customers Churn Prediction Model

Power Co Churn Analysis
Powerco is a major gas and electricity utility that supplies corporate, SME (Small & Medium enterprises), and residential customers. The power liberalization of the energy market in Europe has led to significant customer churn, especially in the SME segment. They have partnered with BCG to help diagnose the source of churning SME customers.
A fair hypothesis is that price changes affect customer churn. Therefore, it is helpful to know which customers are more (or less) likely to churn at their current price, for which a good predictive model could be useful.



<img width="600" height="401" alt="image" src="https://github.com/user-attachments/assets/3e81fe88-3b3f-471c-93f9-436fad2618f6" />


Project Objectives:
How to investigate whether price sensitivity is the most influential factor for a 
customer churning.
To Predict Customers likely to churn based on historical data. 
Improve Customer Retention by implementing proactive and personalised interventions to reduce churn.
Strengthen Customer relationships to sustain business growth.


Data Description
client_data.csv 

● id = client company identifier 

● activity_new = category of the company’s activity

● channel_sales = code of the sales channel

● cons_12m = electricity consumption of the past 12 months

● cons_gas_12m = gas consumption of the past 12 months

● cons_last_month = electricity consumption of the last month 

● date_activ = date of activation of the contract

● date_end = registered date of the end of the contract

● date_modif_prod = date of the last modification of the product 

● date_renewal = date of the next contract renewal

● forecast_cons_12m = forecasted electricity consumption for next 12 months ● forecast_cons_year = forecasted electricity consumption for the next calendar year 

● forecast_discount_energy = forecasted value of current discount

● forecast_meter_rent_12m = forecasted bill of meter rental for the next 2 months 

● forecast_price_energy_off_peak = forecasted energy price for 1st period (off peak)

● forecast_price_energy_peak = forecasted energy price for 2nd period (peak) ● forecast_price_pow_off_peak = forecasted power price for 1st period (off peak)

● has_gas = indicated if client is also a gas client 

● imp_cons = current paid consumption 

● margin_gross_pow_ele = gross margin on power subscription 

● margin_net_pow_ele = net margin on power subscription

● nb_prod_act = number of active products and services 

● net_margin = total net margin 

● num_years_antig = antiquity of the client (in number of years)

● origin_up = code of the electricity campaign the customer first bed to

● pow_max = subscribed power

● churn = has the client churned over the next 3 months 


Exploratory Data Analysis
Key findings:
 About 9.72% of customers changed providers.
 Numeric variables on consumption are highly skewed.
 Changes in prices do not affect customer churn.



Feature Engineering
Created tenure groups to categorise customers by their duration with PowerCo.
Irrelevant or multicollinear features such as num_years_antig and forecast_cons_year were dropped
Categorical variables were encoded, and synthetic samples were generated using SMOTE-ENN for class balance

Machine Learning Model
Logistic Regression
Decision Tree
Random Forest
Precision: 92.3076923076923%
Accuracy: 90.08762322015335%
Recall: 3.2171581769436997%

Recommendations
Based on insights from the analysis:
Develop Targeted retention strategies that focuses on at- risk customers based on model prediction,
Monitoring the effectiveness of the discount towards reducing churn and optimising retention.
Optimise Marketing Spend by allocating  resources to retention efforts with the highest impact.
Continuous Monitoring  regularly to evaluate and update the model to maintain effectiveness.

Conclusion
 This project provides a robust, data - driven solution for mitigating customer churn at PowerCo. It combines advanced analytics and machine learning to proffer actionable insights and effective strategies to improve customer retention and strengthen PowerCo market position. 



