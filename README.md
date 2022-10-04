# my_lamba_deployment---project-2

Project #2 - Pixelator 

Completed following Adrian Catnrills AWS Hands on Demos - https://learn.cantrill.io/p/labs-overview 


This Project consists of a simple event-driven image processing pipeline.

1) The pipeline involves two S3 buckets - a source bucket and a processed bucket. 
2) Once images are uplaoded to the source bucket a lamba function is triggered based on the PUT action.
3) The Lambda function will then recieve the event and extract bucket and object information.
4) Once those details are known, the lambda function using the PIL module pixelates the image with 5 seperate variations and uploads into the processed bucket 
(8x8, 16x16, 32x32, 48x48 and 64x64)
