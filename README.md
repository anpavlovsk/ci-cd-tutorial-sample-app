[![Test and build Docker Image](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/test_and_build.yml/badge.svg?branch=main)](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/test_and_build.yml)
[![Deploy to Dev Environment](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/dev.yml/badge.svg?branch=main)](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/dev.yml)
[![Deploy to Prod Environment](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/prod.yml/badge.svg)](https://github.com/LygutaKsusha/ci-cd-tutorial-sample-app/actions/workflows/prod.yml)
[![Quality gate](https://sonarcloud.io/api/project_badges/quality_gate?project=application-ksu)](https://sonarcloud.io/summary/new_code?id=application-ksu)

# CD/CI Tutorial Sample Application

## Description

This sample Python REST API application was written for a tutorial on implementing Continuous Integration and Delivery pipelines.


It demonstrates how to:

 * Write a basic REST API using the [Flask](http://flask.pocoo.org) microframework
 * Basic database operations and migrations using the Flask wrappers around [Alembic](https://bitbucket.org/zzzeek/alembic) and [SQLAlchemy](https://www.sqlalchemy.org)
 * Write automated unit tests with [unittest](https://docs.python.org/2/library/unittest.html)

Also:

 * How to use [GitHub Actions](https://github.com/features/actions)

Related article: https://medium.com/rockedscience/docker-ci-cd-pipeline-with-github-actions-6d4cd1731030

## Installation

How set up and run application you may find with the initial link of the root repo 
https://github.com/edonosotti/ci-cd-tutorial-sample-app

## CI/CD Workflow
This repo shows basic set up of the CI/CD Workflow with Github Actions

## Features:
- Reusable action workflows, that can be called from previous one
- Deploy to Prod workflow also requires manual approval in addition, after all previous checks and builds were completed and passed
- The application is deployed to AWS using ElastickBeanstalk service
Url links for Dev and Prod apps basic functionality response are available here:
http://test-environment.eba-kupdirkf.us-east-1.elasticbeanstalk.com/
http://productionenv-env.eba-j3j3u7ux.us-east-1.elasticbeanstalk.com/
- Application's built versions are stored as artifacts in the Docker Hub
Image is available here 
https://hub.docker.com/repository/docker/ksusha/dockerhub-actions-eks
- Project is scanning with SonarCloud (https://sonarcloud.io/)
Link to the scan results is available here
https://sonarcloud.io/component_measures?id=application-ksu&branch=main
https://sonarcloud.io/project/overview?id=application-ksu
- Status response messages are getting to Slack channels

