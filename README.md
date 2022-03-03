### Problem Statement
Disease can change the picture  of world. As we saw that covid have shaken the world and took millions of lives.in 2019 and 2020 gdp of all the country decrease significantly and now the death rate of covid reduced and gdp become normal again.but the cost of product increased around 1.2 times.

so in this projects i will try to find if there any relationshp with death rate by desease and gdp. i will also analyse last 30 year data of death by desease. i will make aa time series model that will help predict future gdp. 



## Data dictionary

1. 30 year data of death by disease
2. 1950 to 2021 year gdp data of USA
3. Population data of all country of 1990 to 2019
4. 30 year cancer death by dype data of all country



|**index|Column|data_shape|data type|Description**|
|---|---|---|---|---|
|0|country|8590 non-null|object|asd|
|1|code |6206 non-null |object |Three dogot country code |
|2|year|8590 non-null|int64|years from 1990 to 2019| 
|3|   meningitis|                   8220 non-null  | float64|death caused by meningitis|
 |4|   neoplasms |                   8220 non-null  | float64|death caused by cancer|
| 5|   fire_heat_hot_substances|      8220 non-null   |float64|death caused by fire or heat substance|
 |6|   malaria|                       8220 non-null   |float64|death caused by malaria|
| 7|   drowing |                      8220 non-null  | float64|death caused by drowing|
| 8 |  interpersonal_violence |       8220 non-null  | float64|death caused by interpersonal violance|
| 9  |hiv_aids                |      8220 non-null  | float64|hiv_aids|
| 10|  drug_use_disorders      |      8220 non-null|   float64|drug disorder|

Also there in 22 more disease data were on the datasets




## Summary
For this project my main goal was to see if their relationship in death rate by disease and gdp. to do that frist i download data from our world in data website where i found 30 years of death by desease data by country. i also wanted to check the disease rate by population of those country so i got another datasets of 30 years of population by country. i also wanted to focus on cancer data so i collected cancer death rate by cancer type of 30 years. frist i merged population and gdp data with disease. i did unsupervised learning and by using k means clusturing i was able to separate data by 4 groups. each group contain data of countries with low death rate by disease. 

for time series model i used lasr 72 years of gdp data of usa. data was collected quarterly (once in every 4 month). i have used arima model to predict future gdp for coming years. there was seasonality. its seems like in every 5 years the gdp go little bit down and then folowing year its increase.  there was linearity in gdp data. it increasing day by day. 

i also run classification model to predict gdp. i took the mean value of gdp and assinged if bigger then mean as yes and less then mean no. (develop vs undeveloped). i have tried 8 model and most of them have accuracy score 90 percent and up. my best model was random forest with 99 percent accuracy on test and train. crossval score precision and recall score was 98 up.


## Conclusion and recommendations

We can conclude that from cardiovascular and lower respiratory infection people are dying much more than other disease. If we compare the death rate from 1990 to 2019 we can see that some disease death rate are decreasing and some of them are increasing. The percentage of death by cancer , liver disease, cardiovascular, diabetes are increasing day by day. And death rate from disease like Malaria, diarrhea is decreasing all over the world. 
Most of the developed country have high death rate from cancer, cardiovascular , alzheimer's disease , parkinson’s disease and very low in diarrhea, malaria. 

Egypt is the only country who has highest liver cancer death and in all the country lung cancer is deadliest. America and Russia have highest death rate in drug use disorder. in USA in every 100k people about 563 cases of cancer and about 185 people die. Bulgaria have highest death rate by cardiovascular disease. 

