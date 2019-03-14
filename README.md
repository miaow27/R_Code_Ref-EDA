# What is this repo for? 

Include all functions created for past EDA, might be useful for future. 

## 1. EDA toolkit
contains a R markdown file with function & Example (Use-case). 
- calculate geo-distance using lat and long


## 2. Cln Date Example
contains R script example for the following typical date transformation problem: 

#### Data Taks: 
Imageine the data looks like this: 

| member ID | start date | end date | enrolled plan |
| ------ | ------ | ------ | ------ |
|A |2015-01-01| 2019-12-31| Atena|
|B | 2015-01-01|2017-03-31| BCBS |
|B | 2018-02-01|2019-12-31| Atena |

And we want to reformat to something like this: 

|member ID| month | enrolled plan| 
| ------ | ------ | ------ |
|A | 2015-01 | Atena|
|A | 2015-02 | Atena |
.....

#### Data Challenge:
Besides the date transformation, the data is extremely big (10 GB) in total. 
And the data analyst have breakdown the data annually for you. 
What should you do if you are interested in knowing the 10-year enrollment/churn infromation? 




