# TensorIoT
TensorIot Interview Assessment
This script is created as part of technical Assessment for the company "TensorIoT".

Actions to be perfomed:
  Download the data files from here - http://jmcauley.ucsd.edu/data/amazon/links.html
  Apache spark tools locally and necessary tools
  Download a review file with a million reviews
  Using Jupyter notebook create a program to read the million reviews and get the following 
  Items having the least rating 
  Items having most rating
  Item having the longest reviews
  Transform: change the date MM-DD-YYYY format
  Show a desired data frame operation which you learnt recently
  Convert the whole file into Parquet file after transforming. 
  Upload code to Github  and complete Readme.md which anyone can understand
  Send Github link to HR Mail ID
  
Solution:
  -Used sparkContext.addFile(url) so as to read data directly from link to save time of upload and download.
  -Used from_unixtime to convert time to MM-DD-YYYY format
  -Used length function get length of Review Text
  -aggerated the min value of ratings to get table of items with least rating.
  -aggerated the max value of ratings to get table of items with most rating.
  -aggerated the max value of ratings to get table of items with max  review length.

Table Contents:
  reviewerID - ID of the reviewer, e.g. A2SUAM1J3GNN3B
  asin - ID of the product, e.g. 0000013714
  reviewerName - name of the reviewer
  helpful - helpfulness rating of the review, e.g. 2/3
  reviewText - text of the review
  overall - rating of the product
  summary - summary of the review
  unixReviewTime - time of the review (unix time)
  reviewTime - time of the review (raw)

