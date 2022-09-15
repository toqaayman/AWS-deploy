## Udagram Pipeline
![Pipeline]([Diagrams/pipeline.png](https://github.com/toqaayman/AWS-deploy/blob/main/Diagrams/pipeline.png))
# Pipeline process

Our process may be summed up in a few stages:
1. The developer updates the codebase in the local environment.
2. When modified code is posted to github, circleci does certain activities.
    1. Setup node/aws-cli/aws-eb-cli
    2. Install front-end dependencies
    3. create a front-end
    4. Install back-end dependencies
    5. create a back-end
    6. Update the elastic-beanstalk back-end code
    7. make changes to the front-end code in its S3 bucket
