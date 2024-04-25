# technical_portfolio  

## 기술 평가 항목
1. Python, SQL, R, Java, Scala, Go, C/C++, Javascript 등 데이터 처리 언어 활용 능력
5. 데이터사이언스 관련 공모전 참여를 통한 공개 데이터의 활용 및 분석 능력
8. R, Python, Tableau, Power BI 등을 활용한 데이터 시각화 능력
---
## 레포지토리 소개
본 레포지토리는 KAMP에서 제공하는 에너지(전력) 사용량 데이터를 활용해 공장에서 관측된는 다양한 변수에 대해 전기 사용량을 예측하는 모델을 학습하고, 결과의 분석 내용을 정리한 것입니다.

---
## 데이터셋 설명
PROBLEM DEFINITION
Within the realm of factory manufacturing, diverse resources including labor, infrastructure, and electrical utilities are expended. Ensuring the optimal utilization of these resources is mandatory.
KEPCO (Korea Electric Power Corporation)* (which is the provider of the dataset of the research) calculates electricity prices based on the maximum power demand. The maximum power demand, also known as the peak demand, refers to the power accumulated in a predetermined time unit through transformers installed in a factory. Maximum power demand is calculated to be prepared for scenarios like facility failures and the sudden use of high-capacity equipment. This calculation involves finding the average power over a predetermined specific time period. In the case of KEPCO, this time period is 15 minutes.
KEPCO monitors the three-month maximum power demand pattern and charges electricity fees by applying the base rate for the next year based on the highest maximum demand power. Therefore, it is important to efficiently manage the maximum demand power from the perspective of the company. If the maximum demand power increases, it leads to an increase in operating costs and acts as a factor in increasing the cost of the company.
DATA DESCRIPTION
The dataset, provided by KEPCO, is collected from the transformer detection sensors of a factory during the manufacturing process at 15-minute intervals. First, we should state that 15mins, 30mins, 45mins, 60mins, and average columns are the dependent variables and all the other columns are independent variables. The values in the dependent columns exhibit correlations with the values in the independent columns.
Now, let us look at the meaning of each column.
date : Operation date, it starts with 1st of January, 2021 and goes until 14th of September, 2021
hour : Operation hour
15mins : Maximum power usage for the first 15 minutes of the hour
30mins : Maximum power usage for the 15-30 minutes of the hour
45mins : Maximum power usage for the 30-45 minutes of the hour
60mins : Maximum power usage for the 45-60 minutes of the hour
average : Average of the 15mins, 30mins, 45mins, and 60mins values
production : Production value to be produced at the corresponding time
temperature : Temperature at the corresponding time
wind_speed : Wind speed at the corresponding time
humidity : Humidity at the corresponding time
rainfall : Amount of rainfall at the corresponding time
electricity_bill_by_season : Electricity bill for the season, it has 3 different values because the dates in the data contain only winter, spring, and summer seasons. This is because the dates in the data are until 14th of September.
day_of_the_week : It has values from 1 to 7 and these numbers represent the day of the week
day : It represents which day of the month it is
month : It represents which month of the year it is
num_of_workers : It represents the manpower that was used that day
personnel_expenses : Ratio of night and day labor costs

## 시각화
Visualization.ipynb에 관련 내용이 정리되어 있습니다.
