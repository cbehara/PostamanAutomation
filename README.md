# data-api-automation-test
[![](https://img.shields.io/badge/license-Siemens%20Inner%20Source-blue.svg)](https://code.siemens.com/siemens/code/blob/master/LICENSE.md)

Postman collections for Data-API

## 1. Collections 

There are 1 Postman Collections in the repository which conatins two subfolders under V1 floder

# IntermediatecData
# Meta Data
# Historical Data
# Online Data

The first folder that needs to be run, in order to subscribe the topics and featch the data from mongoDB as per the key value.
The Second folder that needs to be run, in order to fetach the medataData as per the TMS,Objecttype and Locode.

Import the Collections into your Postman Client:

* DataApi_Postman_Collection 


## 2. Environments 
Import the Environment Config and make rhe required changes to reflect the correct endpoints to the Data API  deployment required to be tested. This environemt file contains all the required variables and placeholders needed by all the collections, but the examples for endpoints provided, point to a local Data API installation with the standard Ingress exposed local endpoints:

[Local Development](url)


## 3. Testing 

The collections can be run as they are via Postman but for a more detailed setup of a complete stand-alone test environment (QA and Regression Testing Framework) please refer to the detailed explanation in the Data-API documentation here


## 4. Support Scripts for Docker-Image 

Refer to their respective onboarding guide for more information.


## 4.1 Prerequisites  

Install Postman CLI Newman:

Ensure that you have NPM installed.

# Install newman
npm install -g newman


## 4.2 Pre-loading Test Data 

Note: Ensure that you execute the following commands in your project folder after running npm install. Note: Ensure that you are in the project root folder

## 4.3 Run the Postman collection using newman command line 

newman run https://www.getpostman.com/collections/09592f2bd6ca698768fd -e DataAPILocalhost_postman_environment.json -d data1.json

## Test Report 

->If you run the postman collection through Newman command line in local , check the HTML report in  project location under Newman report folder
-> if your the postaman collection through Gitlab runner , check the HTML report under artifacts 
-> Test Report which contains the collection information , Test Cases passed , Test Cases failed  and Test Cases skipped 

## License
Code and documentation copyright 2020 Siemens AG.
See [LICENSE.md](LICENSE.md).


## Maintainer
Chakravarthi Behara

 