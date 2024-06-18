# Test API SoapUI Project

This repository contains a REST project constructed using the `SoapUI` tool. The `TestSuite` is designed by TestCases: Create Pre-requests, Operate by Space Tags, Delete Pre-requests. 
And the same ensuring efficient and comprehensive testing of all API endpoints as specified in the ClickUP API requirements to [GetSpaceTags](https://clickup.com/api/clickupreference/operation/GetSpaceTags/).

## Table of Contents
1. Setup local machine<br/>
2. Prerequisites<br/>
2. Run the Collection<br/>

## 1. Setup local machine
#### This guide assumes the following:
* Have **SoapUI** version 5.7.2 or higher installed on your system

## 2. Prerequisites:
#### Before proceeding, ensure you have the following:
* Basic understanding of Groovy scripting
* Knowledge of JSON schema validation concepts

#### JSON schema validation in SoapUI
This guide will walk you through the process of setting up JSON schema validation in SoapUI for POST methods using Groovy script with the `json-schema-validator` library:
1. Go to the [Maven Repository](https://mvnrepository.com) and download the [`json-schema-validator-2.2.12`](https://repo1.maven.org/maven2/com/github/java-json-tools/json-schema-validator/2.2.12/) jar file along with all its dependencies: [`json-20240303`](https://repo1.maven.org/maven2/org/json/json/20240303/), [`jackson-databind-2.17.1`](https://repo1.maven.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.17.1/), [`jackson-core-2.17.1`](https://repo1.maven.org/maven2/com/fasterxml/jackson/core/jackson-core/2.17.1/) jar files.
2. Find the directory where SoapUI is installed on your system. For example, it could be `/Applications/<SOAPUI_APP_NAME>/` (for macOS). Inside the SoapUI installation directory, locate the `ext` directory and copy the all downloaded jar files into this directory.
3. Restart SoapUI to update the libraries and enable the newly downloaded jar files.
4. Run the test. Execute the POST method test in SoapUI to trigger the JSON schema validation through your Groovy script. Check the test results to ensure that the JSON response schema is validated successfully.

## 3. Run the Collection
* Import project.
* Use the SoapUI TestSuite Runner to execute the project, ensuring the pre- & post- scripts are executed to maintain data integrity.
