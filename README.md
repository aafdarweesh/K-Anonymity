# K-Anonymity
### Description 
In the project the K-Anonmity is applied for the Attached Data: adult.csv
Using ARX platform. References:
```
ARX lib: https://arx.deidentifier.org/
K-anonymity : https://en.wikipedia.org/wiki/K-anonymity
 
```

## Configurations
According to the data the following descisions were made

1) Age: Intervals as it makes more sense as masking is not an option as it will give an indication

2) workclass: found that private category has many attributes, so I put it in a section and grouped the government together, and the rest in self-emp (will check it later, might need to add self-emp to government if they are very small)

3) fnlwgt "Final weight income": Intervals as masking will not be an option, as there is one entry with prefix 18*** (according to the data, the interval decided to be 10,000)

4) Education: Grouping together, to 3 main categories (school, uni, post grad)

5) Education Number: Interval of 10 as 9 & 10 have the highest numbers alone, and I want each to be in a separate group

6) Marital: to 3 categories according to the representation in the data, as devorced/widow/separated have relatively low each but related and around 30% together, the same apply for Maried. However, Nevermarries is already high ~30%

7) Occupation: Grouped into 3 : Technical, Non-Technical, Others

8) Relationship: Grouped into Spouse and Other. As Wife data was small in size and other-relatives

9) Race was generalized as some races are really really small in data size

10) Gender: was generalized to person

11) capital-gain: was identifier to some entries to cateforized as identifier

12) capital-loss: was identifier to some entries to cateforized as identifier

13) hours per week: was grouped into 2 categories as 40hours had 80% of the data

14) native country was categorized according to the Continent

15) Income: was categroized into two categorizes as it was.

## Findings
### Data & Configurations
![Alt text](./README_pictures/Data.png?raw=true "Search Bars")
### Result Exploration
![Alt text](./README_pictures/Result_Explore.png?raw=true "Search Bars")
### Analyse Risk Result
![Alt text](./README_pictures/Risk_Tests.png?raw=true "Search Bars")
### Analyse Risk Tests
![Alt text](./README_pictures/Risk_Graph.png?raw=true "Search Bars")
