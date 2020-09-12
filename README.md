## Build CI/CD Pipelines, Monitoring, and Logging
This repository provides the supporting material for the "ND9991 Cloud DevOps Nanodegree - C3 - Build CI/CD Pipelines, Monitoring, and Logging" course. This repo has two more branches, other than the master branch.

* Blue/Green branch corresponds to the Blue/Green deployment strategy. Make sure that you checkout branches "blue" and "green" to see how blue/green deployment was performed in the course.
* You can create any more branches for a multiple pipeline set-up, as directed in the demonstration video.

### Dependencies
##### 1. AWS account
You would require to have an AWS account to be able to build cloud infrastructure. Particularly, you will need to create S3 buckets, EC2 instances, and IAM users.

#### 2. Jenkins on Ubuntu VM
As a part of the project, you will need to install Jenkins and a few plugins to assist your requirements, as mentioned in the "Jenkins Pipelines on AWS --> Project Details" page in the classroom.

## Prerequisite
1. A little knowledge of basic commands in Unix terminal.
2. Understanding of software testing frameworks - JMeter and JUnit
3. Understanding of deployment strategies

## Challenges
1. Install Tidy on linux server.
2. Integrate with AWS S3

## Project Steps:

Copy the IAM User sign-in link from the IAM Dashboard.
https://777933753083.signin.aws.amazon.com/console


## Deployment Strategies
Deployment strategy is an approach to roll out the updates/changes made in the "live" application. The idea is that the application must not be brought down to introduce the updates. There are a variety of strategies available. Let's assume that there are two versions of the software applications - version A and B. Version B is the updated version.

1. Rolling - Version B is gradually rolled out succeeding version A. This is suitable when the updates are very small, such as bug fixes.
2. Blue/Green - Version B is released alongside version A, then the traffic is switched to version B. This is the preferred model when there are major updates or releasing new features.
3. Canary - Version B is released to a specific subset of users for early feedback and testing, then proceed to a complete rollout.
4. A/B testing - Version B is released to a subset of users under particular conditions.
5. Recreate - Version A is terminated first, and then the version B is rolled out.
6. Shadow - Version B receives real-world traffic alongside version A and doesn’t impact the response.

## Supporting links
https://www.jenkins.io/doc/tutorials/build-a-multibranch-pipeline-project/#create-your-pipeline-project-in-blue-ocean
https://wiki.jenkins.io/display/JENKINS/How+to+run+JMeter+with+Jenkins
https://plugins.jenkins.io/junit/
https://www.jenkins.io/doc/pipeline/steps/junit/
https://docs.ansible.com/ansible/latest/index.html
https://github.com/jenkinsci/pipeline-aws-plugin#withaws
https://github.com/jenkinsci/pipeline-aws-plugin#s3uploadhttps://docs.aws.amazon.com/AmazonS3/latest/dev/access-policy-language-overview.html
https://docs.aws.amazon.com/AmazonS3/latest/dev/access-policy-language-overview.html
