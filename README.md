{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "24a60a5c-6a9d-4c18-a1b2-e7268a82771e",
   "metadata": {},
   "source": [
    "### Problem Statement\n",
    "Disease can change the picture  of world. As we saw that covid have shaken the world and took millions of lives.in 2019 and 2020 gdp of all the country decrease significantly and now the death rate of covid reduced and gdp become normal again.but the cost of product increased around 1.2 times.\n",
    "\n",
    "so in this projects i will try to find if there any relationshp with death rate by desease and gdp. i will also analyse last 30 year data of death by desease. i will make aa time series model that will help predict future gdp. \n",
    "\n",
    "\n",
    "\n",
    "## Data dictionary\n",
    "\n",
    "1. 30 year data of death by disease\n",
    "2. 1950 to 2021 year gdp data of USA\n",
    "3. Population data of all country of 1990 to 2019\n",
    "4. 30 year cancer death by dype data of all country\n",
    "\n",
    "\n",
    "\n",
    "|**index|Column|data_shape|data type|Description**|\n",
    "|---|---|---|---|---|\n",
    "|0|country|8590 non-null|object|asd|\n",
    "|1|code |6206 non-null |object |Three dogot country code |\n",
    "|2|year|8590 non-null|int64|years from 1990 to 2019| \n",
    "|3|   meningitis|                   8220 non-null  | float64|death caused by meningitis|\n",
    " |4|   neoplasms |                   8220 non-null  | float64|death caused by cancer|\n",
    "| 5|   fire_heat_hot_substances|      8220 non-null   |float64|death caused by fire or heat substance|\n",
    " |6|   malaria|                       8220 non-null   |float64|death caused by malaria|\n",
    "| 7|   drowing |                      8220 non-null  | float64|death caused by drowing|\n",
    "| 8 |  interpersonal_violence |       8220 non-null  | float64|death caused by interpersonal violance|\n",
    "| 9  |hiv_aids                |      8220 non-null  | float64|hiv_aids|\n",
    "| 10|  drug_use_disorders      |      8220 non-null|   float64|drug disorder|\n",
    "\n",
    "Also there in 22 more disease data were on the datasets\n",
    "\n",
    "\n",
    "\n",
    "\n",
    "## Summary\n",
    "For this project my main goal was to see if their relationship in death rate by disease and gdp. to do that frist i download data from our world in data website where i found 30 years of death by desease data by country. i also wanted to check the disease rate by population of those country so i got another datasets of 30 years of population by country. i also wanted to focus on cancer data so i collected cancer death rate by cancer type of 30 years. frist i merged population and gdp data with disease. i did unsupervised learning and by using k means clusturing i was able to separate data by 4 groups. each group contain data of countries with low death rate by disease. \n",
    "\n",
    "for time series model i used lasr 72 years of gdp data of usa. data was collected quarterly (once in every 4 month). i have used arima model to predict future gdp for coming years. there was seasonality. its seems like in every 5 years the gdp go little bit down and then folowing year its increase.  there was linearity in gdp data. it increasing day by day. \n",
    "\n",
    "i also run classification model to predict gdp. i took the mean value of gdp and assinged if bigger then mean as yes and less then mean no. (develop vs undeveloped). i have tried 8 model and most of them have accuracy score 90 percent and up. my best model was random forest with 99 percent accuracy on test and train. crossval score precision and recall score was 98 up.\n",
    "\n",
    "\n",
    "## Conclusion and recommendations\n",
    "\n",
    "We can conclude that from cardiovascular and lower respiratory infection people are dying much more than other disease. If we compare the death rate from 1990 to 2019 we can see that some disease death rate are decreasing and some of them are increasing. The percentage of death by cancer , liver disease, cardiovascular, diabetes are increasing day by day. And death rate from disease like Malaria, diarrhea is decreasing all over the world. \n",
    "Most of the developed country have high death rate from cancer, cardiovascular , alzheimer's disease , parkinson’s disease and very low in diarrhea, malaria. \n",
    "\n",
    "Egypt is the only country who has highest liver cancer death and in all the country lung cancer is deadliest. America and Russia have highest death rate in drug use disorder. in USA in every 100k people about 563 cases of cancer and about 185 people die. Bulgaria have highest death rate by cardiovascular disease. \n",
    "\n",
    "\n",
    "\n",
    "\n",
    "```python\n",
    "\n",
    "```\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ad6adbf1-945b-4233-a025-6bf030468960",
   "metadata": {},
   "source": []
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "a94e1d61-0ee3-47e4-8fc8-d07b6a978616",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
