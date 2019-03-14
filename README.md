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
Notice when you turn the data into the "long format", the data will become even bigger since you will create 10 rows for 10 months. This is becuase the "long" format is more desireable for analysis purpose. 

In my case, the raw data is about 8GB while after the transformation it becomes 20GB. 
Remembere that R can take 2^31 data element but since this data is extremely "long" and we have 4 coloumns, it can only take 10 million people for 50 months. And this does not work for me becuase I have more than 15 million popultion.




