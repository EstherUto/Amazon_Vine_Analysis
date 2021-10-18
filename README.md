# Amazon Vine Analysis

## Table of Contents
- [Overview of Analysis](#overview-of-analysis)
- [Results](#results)
- [Summary](#summary)

## Overview of Analysis

The purpose of this analysis was to analyze Amazon reviews written by members of the Amazon Vine program. The Amazon Vine program is a service that allows sellers to receive reviews on their products. There are multiple [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) publicly available to download. For this particular project, Baby Products reviews data was utilized. It is important to note that Vine is a paid service and there are reviews from non-Vine (unpaid) customers.

## Results

The data set contained about 1,700,000 reviews from different customers, however for this simple analysis, the focus was on manufacturers who had 20 or more reviews, narrowing the scope to just over 25,000 manufacturers.

Out of all the reviews deemed helpful (i.e. percentage of helpful votes to total votes >= 50%) there were a total of 446 Vine manufacturers and over 23,000 non-Vine manufacturers. Figure 1 and Figure 2 provide a snapshot of the resulting dataframe including the number of reviews.

**_FIGURE 1. Vine Reviews_**

<img width="427" alt="Vine" src="https://user-images.githubusercontent.com/86085601/137649894-090c8170-3b15-4a39-99d9-f7134021c5e8.png">

**_FIGURE 2. non-Vine Reviews_**

<img width="427" alt="non-Vine" src="https://user-images.githubusercontent.com/86085601/137649896-8dd8ce7e-7f35-4292-9b08-8520dcae5027.png">

From our set, there were a total of 11,679 five star reviews, however, the Vine manufacturers accounted for only 1.67% (195) of those reviews while non-Vine manufacturers represented over 97% (> 11,000) of five star reviews. This may be due to a variety of reasons such as there are less Vine manufacturers overall or the general public being more likely to buy from non-Vine manufacturers. 

Over 24,000 reviews have a helpful rate of 50% or higher, meaning the reviews either helped being a deciding factor on purchase, or the review was on point on the critique of the product.

## Summary

Five star ratings account for at least 45% of total ratings, however, this alone cannot determine if there is positivity bias in the reviews. To have positivity bias, it is safe to mention five star ratings would have to account for 75% or higher of reviews. In both cases of Vine and non-Vine reviews, five star ratings were also approximately 45% so it cannot be said there is some sort of positivity bias.

To analysis to be done to fully comprehend if there is positivity bias would be to look into how many helpful votes were from verified purchases and how long those verified purchasers have had their product. This would help to understand if there is some sort of bias in the reviewing of the product.
