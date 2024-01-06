# YouTube Data Analytics using AWS Glue, Lambda, and Athena
## Dataset Description:
This dataset includes several months (and counting) of data on daily trending YouTube videos. Data is included 
from the US, GB, DE, CA, and FR regions (USA, Great Britain, Germany, Canada, and France, respectively), 
with up to 200 listed trending videos per day.
Each region’s data is in a separate file. Data includes the video title, channel title, publish time, tags, views, likes 
and dislikes, description, and comment count.
The data also includes a category_id field, which varies between regions. To retrieve the categories for a specific 
video, find it in the associated JSON. One such file is included for each of the five regions in the dataset.

## Summary:
In this project we aim to securely manage, streamline, and perform analysis on the structured and semi-structured 
YouTube video data based on the video categories and the trending metrics. We first load the dataset onto an 
AWS S3 bucket. To process the given data properly, we would require doing certain transformations on the data. 
We would achieve this using Glue ETL and AWS Lambda. Once we get the cleaned and transformed data, we 
will store it in another bucket. Finally, we would join the two separate tables resulting from the above steps, to 
create the final table. We would also follow this by visualizing the data created using AWS QuickSight. The 
project is to do data ingestion then build an ETL system in the cloud and report the dashboard to get the answers 
to the questions asked.

## Cloud Services Used:
Amazon S3: It is for object storage.
AWS IAM: To manage user identities and access to AWS resources.
AWS QuickSight: BI tool build for the cloud.
AWS Glue: Serverless data integration service for ETL jobs.
AWS Lambda: Computing service where we run the code without worrying about managing servers.
AWS Athena: It is used for interactive query for S3 where there is no need to load data and it stays in S3.
