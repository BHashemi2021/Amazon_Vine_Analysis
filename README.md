# Amazon Vine Analysis
Analyzing Amazon reviews by members of its paid Amazon Vine program.

## Background
We have been tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. The [Amazon Vine program](https://www.amazon.ca/gp/help/customer/display.html/?nodeId=GPEWN3RSQPEU2HST&pop-up=1) is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we will have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We will need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we will use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in our dataset. Then, we will write a summary of the analysis for to be submitted to the SellBy stakeholders.

## What We Are Creating
This new assignment consists of two technical analysis deliverables and a written report. We will submit the following:

    Deliverable 1: Perform ETL on Amazon Product Reviews
    Deliverable 2: Determine Bias of Vine Reviews
    Deliverable 3: A Written Report on the Analysis (README.md)
  
### Deliveravle 1
  We created an AWS RDS database with tables in pgAdmin, picked US Amazon reviews of Musical Instruments (v1) dataset available from the [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), and extracted the dataset into a DataFrame (Table 1). We transformed the DataFrame into four separate DataFrames that matched the table schema in our pgAdmin. We later will uploaded the transformed data into the appropriate tables on to the relational database on Amazon Web Serices (AWS) website and ran queries through pgAdmin to confirm that the data had been uploaded.
  
  
  #### Table 1: The dataset in a tabular format
  
  ----------------------------------
  
  ![1.png](https://github.com/BHashemi2021/Amazon_Vine_Analysis/blob/main/Resources/images/1.png)
  
  ----------------------------------
  
  
### Deliveravle 2
Using PySpark, Pandas, or SQL, we determined if there was any bias towards reviews that were written as part of the Vine program. For this analysis, we determined if having a paid Vine review made a difference in the percentage of 5-star reviews.

### Deliverable 3
A summary report of the Vine Review Analysis.

#### Overview of the Vine Review Analysis
Explain the purpose of this analysis.

#### Results: 
Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.


