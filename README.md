# Amazon_Vine_Analysis
 
## Overview of the analysis
This project is meant to show the analysis of amazon reviews written by paid and unpaid members of the amazon vine program. The data set being used here is amazon reviews of "us digital video games." The analysis is created by performing an ETL of this data by using AWS RDS, PgAdmin, and PySpark. Additionally, I determined biasness of vine reviews with the data using PySpark.

## Results

- How many Vine reviews and non_Vine reviews were there?
  - 0 paid and 1685 unpaid reviews

- How many Vine reviews were 5 stars? How many non_Vine reviews were 5 stars?
  - 0 paid 5 star reviews and 631 unpaid 5 star reviews

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - 0 percent of Vine reviews were 5 stars. 37.5% of non-Vine reviews were 5 stars

Below are the calculations:

<img width="347" alt="image" src="https://user-images.githubusercontent.com/104074135/199188937-c7f75032-a3e3-4c42-b3c4-5f04226d2cdc.png">

<img width="374" alt="image" src="https://user-images.githubusercontent.com/104074135/199188987-b277792a-9edc-46d9-8635-f5de6b231e55.png">


Below are the respective data frames for paid and unpaid:

<img width="809" alt="image" src="https://user-images.githubusercontent.com/104074135/199189250-4cca4ab2-55d1-48a5-9bd1-74ee5a7f6ba2.png">

<img width="834" alt="image" src="https://user-images.githubusercontent.com/104074135/199189292-eb2b6138-ec0f-4ea7-bf09-9a1574931fb4.png">


## Summary
This data set is a complete miss on the purpose of this analysis due to there being no "helpful" Vine reviews. What is known, is that 37.5% of non-Vine reviews were 5 stars. Theoretically speaking, if Vine reviews had a significantly higher percentage than non-Vine reviews for 5 star ratings, then there would be a clear bias. It would prove useful to run this analysis on multiple datasets then compare the variance of vine and non-vine 5 star review percentages between sets. Doing that could show that some product reviews are more bias than others. Unfortunately, this data set would skew results as there were no vine reviews.
