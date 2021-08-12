# Amazon_Vine_Analysis

## Overview

This analysis uses PySpark to extract a dataset of Amazon luggage reviews, transform the data, and load the transformed data into pgAdmin. The analysis will also filter and look closer at the data to determine if there is bias toward favorable reviews from paid Vine members within the dataset. 

## Results

Reviews written on Amazon for luggage were extracted and a dataframe was created to pull in any reviews that had more than 20 votes and were voted helpful at least 50% of the time. Those reviews were then split into two dataframes: paid Vines reviews and unpaid reviews. The first 20 rows of each of these dataframes are shown below.

Paid Vines Reviews</br>
![Alt Text](https://github.com/lyanneagger/Amazon_Vine_Analysis/blob/main/Resources/paid_df.png "Paid Vines Reviews Dataframe")</br>

Unpaid Reviews</br>
![Alt Text](https://github.com/lyanneagger/Amazon_Vine_Analysis/blob/main/Resources/unpaid_df.png "Unpaid Reviews")</br>

- There were 21 paid Vine reviews vs. 6690 unpaid reviews.
- There were 10 paid Vine reviews of 5 stars. There were 3448 unpaid reviews of 5 stars.
- Five-star reviews made up 47.6% of the total paid Vine reviews and 51.5% of the unpaid reviews.

## Summary

Within this dataset, there is no bias towards positive paid reviews as opposed to unpaid reviews. The unpaid reviews actually had a higher percentage of 5-star reviews out of a much larger group.

However, a deeper analysis may provide more insight, grouping 4- and 5-star reviews together. At a glance, the paid Vines reviews also have a large number of 4-star reviews. Comparing the grouping to unpaid 4- and 5-star reviews would provide more true insight to any bias that may exist. 

It is also noteworthy that the small total group of paid Vines reviews makes true comparison difficult. 