# **Amazon Vine Analysis  using Spark, AWS, and PostGres**

Analysis of Amazon review dataset using Spark in Google Colab, AWS server and Postgres to determine whether there is a difference in the performance of unpaid reviews and paid reviews as part of the Vine program

## **Resources**
------------------

* Data: Amazon AWS S3 U.S. Luggage Review dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt
*Sofware: Google Colaboratory, AWS RDS and S3, pgAdmin 4 Version 5.5

## **Analysis**
-------------------

Analysis of U.S. Amazon luggage review dataset, which among others includes star rating, number of helpful votes, total votes, and whether or not the review was part of the paid Vine program. Initially filtering for reviews that have received at least 20 votes:

![image](https://user-images.githubusercontent.com/93295751/155925722-58003567-4248-49ff-8526-0a42851b7203.png)

Next filtering for reviews where the share of helpful votes to total votes is at least 50%

![image](https://user-images.githubusercontent.com/93295751/155925767-0d141137-57e6-4ff3-bf1a-a80e17bc4136.png)

## **Results**
-----------------

Splitting those results based on paid reviews which were part of the Amazon Vine Program. As well as regular views not paid for yields the following results: 

![image](https://user-images.githubusercontent.com/93295751/155925941-e2882240-946d-452d-91aa-8bdd684552ec.png)

![image](https://user-images.githubusercontent.com/93295751/155925954-d5da8c62-ac93-4092-a2cb-09858deca6b9.png)

## **Summary**

There appears to be no positivity bias when it comes to the Vine program. In fact, reviewers paid for under the Vine program appear to be more critical of the products than those not paid for reviews. However, the sample size for Vine reviews is very small (only 21 reviews were found after the original filtering methods were applied), compared to nearly 6,700 regular reviews.

Further analysis could include a statistical analysis to determine whether the results are statistically significant. The restrictions for the initial criteria could also be loosened, for example by counting all reviews that received at least 10 votes. That would allow for further analysis to determine whether paid reviews are less likely to be deemed helpful or voted on.
