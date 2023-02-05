# AWS_EMR_HIVE_QUICKSIGHT_PIPELINE
Demonstrates working of hive on aws emr,Visualise the data using aws QuickSight

Architecture of the project:

![architecture](https://user-images.githubusercontent.com/70155167/216805531-5b4bdc04-5be0-42d8-9673-1ba4d167fc05.png)





  Code Flow:

    - Create one S3 bucket in the US East Region
    - Load sample CSV using AWS CLI to S3 bucket.
    - Create a 1 m5xLarge EMR instance in the US East Region.
    - Login to EMR instance using Key Pair (passwordless)
    - Create an aggregate table using HiveQL in EMR and store the result back to S3.
    - Read the aggregate table result in Hue and Athena.
    - Generate Chart from Aggregated table using AWS QuickSight.
