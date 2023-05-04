# Hosting a Full-Stack Application
## Intro

   This project is related to my Advanced Full-Stack Web Development Nanodegree Program where I was given a local web application and I was asked to deploy it using aws 
   services through analyzing the technology used to develop the app including programming language, packages used, needed components.My work is code is the package.json 
   added scripts for deployment, software architecture diagram design and config.yml file for creating the pipeline. 

---

## Screenshots
### diagrams
1. software architecture diagram
<p float="left">
  <img src="https://github.com/abdelrahman32002/Web-App-Deployment/blob/main/screenshots/architecture-diagram.jpg?raw=true" width="700" height="350" />
  <br></br>
 2. Pipeline diagram
 <img src="https://github.com/abdelrahman32002/Web-App-Deployment/blob/main/screenshots/pipline.jpg?raw=true" width="700" height="350" />
 
</p>
### Pipeline
<p float="left">
  <img src="https://github.com/abdelrahman32002/Web-App-Deployment/blob/main/screenshots/sub1.png?raw=true" width="600" height="500" />
 <img src="https://github.com/abdelrahman32002/Web-App-Deployment/blob/main/screenshots/sub2.png?raw=true" width="600" height="500" />
  <img src="https://github.com/abdelrahman32002/Web-App-Deployment/blob/main/screenshots/sub3.png?raw=true" width="600" height="500" />
  </p>
  
  




### Infrastructure

```
- AWS S3 bucket for static web hosting (Front-end)

- AWS RDS using postgresSQL acts as a database

- AWS Elastic Beanstalk Environment which acts as a server for back-end

```

### Runbook

Steps to test project

1. Clone repository to your Github account
1. Open CircleCi
1. Connect your github account to circleci
1. In the project configure your AWS IAM user
1. Go to the project and run the workflow


### Explanation of pipeline

This pipeline first installs node, elasticbeanstalk CLI and aws CLI then it executes the build job which starts by installing the needed packages for backend and front end , also it runs scripts for linting front end and building backend and front end to convert files to javascript. Then the deploy job starts by deploying the backend  on elasticbeanstalk environment then deploying the frontend by sending the files to S3 bucket.



