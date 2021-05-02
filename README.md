#### DeltaX





Filename : this line is added
Comments
Link


data.csv
Raw metrics from 01-Aug-2020 to 28th Feb-2021.
https://s3.amazonaws.com/backup.deltax.com/dump/data.csv 
predict.csv
Your model needs to predict for these data points.
https://s3.amazonaws.com/backup.deltax.com/dump/predict.csv 
sample_submission.csv
Contains column format for the submission of assignment - submission.csv file. Your model needs to predict for columns (impressions, clicks, conversions, revenue) using input data points from predict.csv
https://s3.amazonaws.com/backup.deltax.com/dump/sample_submission.csv 


**
About the Data**
The sample data dump shared above is the ad performance for the dates between 1st August 2020 and 28th Feb 2021.

Here is a brief hierarchy for relationships in adtech systems:


One Campaign can have one or more Ad Groups. One Ad group can have one or more ads. In the given
One Campaign can have one or more Ad Groups. One Ad group can have one or more ads. In the given dataset - we have only 1 campaign; 4 Ad Groups and multiple ads.


Here is a brief description of all performance columns in the data set:

Raw metrics:
Impressions - Number of time the ad was shown
Clicks - Number of time the ad clicked shown
Cost - Amount spent to show ad
Conversions - Number of transactions received (higher the better)
Revenue - Total value of transactions received (higher the better)

Efficiency metrics: 
Needs to be calculated and are based on raw metrics
CTR - Clicks / Impression (higher the better - used to evaluate if the users find the ad relevant)
CPC - Cost / Click (lower the better - used to evaluate if the cost for getting a click)
CPA - Cost / Conversion (lower the better - used to evaluate if the cost for getting a conversion)
ROI - Revenue/Cost (higher the better - used to evaluate the effectiveness of the advertising budget spent)

Problem Statement

An advertiser would like to estimate the performance of his campaign in the future.

For the given data, please try to address the below questions:
Perform exploratory data analysis and specify your findings with respect to any trends or outliers based on raw or efficiency metrics
Identify correlation in performance of the ads by time metrics if any (Eg day of the week, day etc)
Given the past performance data, predict the performance (Impressions, Clicks, Conversions, Revenue) of an ad between March 1st and March 15th. Use the data in predict.csv for your predictions and submit your response as shown in the file sample_submssion.csv)
How to Submit Assignment
Keep the subject line of your email as “YOUR NAME - Assignment” eg: “Ram N - Assignment”. 

Note:
Being able to summarise your findings visually is important for us. 
Please use appropriate charts/graphs.
Please write your thought process and findings below the visualization as comments in the Juypter notebook
Your submission.csv will be evaluated using RMSE and R2 metrics. 
The Jupyter notebook that you share with us, should fetch the data directly from the S3 Bucket to the notebook and should be fully executable without any errors.
#Example
data=pd.read_csv("https://s3.amazonaws.com/backup.deltax.com/dump/data.csv ")


We are expecting the following attachments in your submissions:
Resume
Jupyter notebook (.ipynb)
Attach submission.csv file. Your model needs to predict for columns (impressions, clicks, conversions, revenue) using input data points from predict.csv. We have also shared a sample sample_submission.csv format so that you can share appropriately.
