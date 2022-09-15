## Udagram Infrastructure
![Infrastructure](diagrams/Infrastructure.png)
# Infrastructure
Infrastructure mostly makes use of four services.

## RDS
Amazon Web Service is utilised to host the relational database 'Postgres,' which we employ to store app data.
Database URI: `postgresql://postgres:password@database-2.cawh6kunp8i1.us-east-1.rds.amazonaws.com/udagram`

## S3
Amazon Web Services was utilised to host our front-end and store website files and uploaded photographs.
Bucket URL: `http://toqaayman-udagram.s3-website-us-east-1.amazonaws.com/home`

## Elastic beanstack
Amazon Web Service is utilised to host our node application and provides us with a nginx server to which we access from our front-end.
EB URL: `http://udagram-api-dev.eba-b4yayrtx.us-east-1.elasticbeanstalk.com/`

## CircleCI
Any event that occurs in our github repo causes the pipeline to update our code, which is a service supplied for us.