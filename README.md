# Workload - Context Driven Dialog


###Context driven dynamic dialog example implemented in Cloud Foundry

This application demonstrates how to combine **IBM Watson™ Natural Language Classifier** and **Retrieve and Rank** with a rule-based system to offer a context driven conversation solution, full flexibility in terms of code change, empowering the business user to change the conversation flow and recommendations. To learn basic concepts, see [Cognitive concepts 101](https://developer.ibm.com/cloudarchitecture/docs/cognitive-concepts-101/).


----


## Introduction

A sample application has been created so you can deploy it into your personal space 
after signing up for Bluemix. You will attach the **IBM Watson™ Natural Language Classifier** and 
**Retrieve and Rank** services to the application as well as learn to begin using these services.

## What Does the App Do?
**TODO** JEROME/HANS EXPLAIN APP

## Deploying the application
The application can be deployed in two ways:

- Single click deploy via DevOps Services
- Manual push through Cloud Foundry command line client


You will need an account on Bluemix. If you are not already signed up, you can sign up on [https://www.bluemix.net](https://www.bluemix.net)


## Single click deploy via DevOps Services

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/hassenius/dynamic-dialogue)

Enjoy! (note, it may take minute or so for the app to start)


## Manual push through Cloud Foundry commmand line client

The goal is to download the application code from github and push it to Bluemix Runtimes to create a running
application that is bound to and consuming Watson services.

If you do not already have the Cloud Foundry command line client installed an configured, you will now need to 
follow the [instructions here](https://github.com/cloudfoundry/cli)

A reference guide can be found [here](https://new-console.ng.bluemix.net/docs/cli/reference/cfcommands/index.html)



1. Download the application code

     If you have git installed, you can clone the repository

     ```git clone **TODO INSERT URL**```

     or download and extract the [Zip file](https://github.com/hassenius/docs/archive/master.zip)
     
1. Create the services using the **Cloud Foundry command line tool** 

     ```cf create-service natural_language_classifier standard NaturalLanguageClassifier```
     
1. Push the Python application

     ```cf push```

     This will push the application as specified in the manifest.yaml file
     
     When the push is completed the application details will be reported, including the randomly generated URL. 
     Navigate to this URL to view and use the application.
    


**TODO**
Deside if ODM files should be included here, if so add explanations. If not find a new home for them, and maybe mention/link from here.
