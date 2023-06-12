# AWS Experiment with Zappa and Flask

This repository contains a Flask-based web application that's designed to experiment with AWS lambda functions and the Zappa deployment framework.

## Project Description

The main goal of this project was to gain a deeper understanding of AWS lambda functions and their potential use cases. After several attempts and much documentation reading, the decision was made to use Zappa, a deployment framework for serverless Python applications on AWS. Zappa simplifies the process of deploying these applications as serverless functions, making it easy to manage and scale the infrastructure.

## About Flask and Zappa

 - **Flask**: Flask is a lightweight and versatile web framework for Python. It is designed to make getting started quick and easy, with the ability to scale up to complex applications.

 - **Zappa**: Zappa is a serverless framework for deploying Python web applications on AWS. Zappa handles all of the configuration and deployment automatically, so you can focus on your application.

## How Zappa Works

Zappa makes it super easy to build and deploy server-less, event-driven Python applications (including, but not limited to, WSGI web apps) on AWS Lambda + API Gateway.

1. **Initialization**: The command **zappa init** is run in the terminal. This command results in the creation of a **zappa_settings.json** file in the project directory. This file houses the configuration details required for Zappa and AWS.

2. **Deployment**: After initialization, the command **zappa deploy dev** is run. This command deploys an application to the AWS Lambda environment. The term 'dev' in this command denotes the environment being deployed to, as per the configuration in the **zappa_settings.json** file.

3. **Updating**: When an application has been modified and requires an updated deployment, the command **zappa update dev** is used. This command updates the deployed application in the AWS environment while maintaining the originally assigned API Gateway URL.
