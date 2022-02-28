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

