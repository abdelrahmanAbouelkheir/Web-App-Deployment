Hosting a Full-Stack Application



---
# Udagram link

http://testing13857395.s3-website-us-east-1.amazonaws.com.


### Runbook

Steps to test project

1. Clone repository to your Github account
1. Open CircleCi
1. Connect your github account to circleci
1. In the project configure your AWS IAM user
1. Go to the project and run the workflow


### Explanation of pipeline

This pipeline first installs node, elasticbeanstalk CLI and aws CLI then it executes the build job which starts by installing the needed packages for backend and front end , also it runs scripts for linting front end and building backend and front end to convert files to javascript. Then the deploy job starts by deploying the backend  on elasticbeanstalk environment then deploying the frontend by sending the files to S3 bucket.

[main](../README.md)
