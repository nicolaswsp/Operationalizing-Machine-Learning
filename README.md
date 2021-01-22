# Operarionalizing Machine Learning in Azure ML Studio

This project aims to demonstrate how to train a model using Azure Machine Learning Studio and put it in production to an end user. The dataset used was Banking Marketing dataset, where the goal is to predict whether a client would sign a bank term deposit based on several features. The training process was made entirely using Auto ML through Azure Machine Learning Studio. After that, it was chosen the best model to accordingly to the best algorithm, VotingEnsemble, and deployed into production. With the deployed model, it was enabled the Application Insight using Azure Python SDK. For the documentation, it was used Swagger instance running with the documentation for the HTTP API of the model. The model was consumed using the deployed scoring URI and key authentication running the endpoint.py script against the API producing JSON output from the model. I was used Apache Benchmark to retrieve the performance result details running against the HTTP API. Finally, it was created, deployed and consumed a pipeline. The model and the pipeline can be accessed through REST terminals.

## Architectural Diagram


The following steps were performed in order to complete this project:

* Authentication
* Automated ML Experiment
* Deploy the best model
* Enable logging
* Swagger Documentation
* Consume model endpoints
* Create and publish a pipeline
* Documentation

## Key Steps
* Registered the Bank Markerting dataset
![picture1](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture1.png)

* Completed the experiment
![picture2](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture2.png)

* Best model obtained by auto ML
![picture3](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture3.png)

* Logs.py were ran obtaining the logs
![picture4](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture4.png)

* The Application Insights was enabled 
![picture5](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture5.png)

* It was ran the Swagger on local host
![picture6](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture6.png)

* Methods and responses from Swagger
![picture7](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture7.png)

  ![picture8](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture8.png)

  ![picture9](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture9.png)

  ![picture10](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture10.png)

  ![picture11](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture11.png)

* Ran the endpoint.py against the API
![picture12](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture12.png)

* Ran Apache Benchmark against the HTTP API
![picture13](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture13.png)

* The pipeline has been created
![picture14](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture14.png)

* The pipeline endpoint is available
![picture15](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture15.png)

* The Published Pipeline overview shows the REST endpoint and the ACTIVE status
![picture16](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture16.png)

* The RunDetails Widget shows the step runs
![picture17](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture17.png)

* ML Studio showing the scheduled run
![picture18](https://github.com/nicolaswsp/Operationalizing-Machine-Learning/blob/main/Images/Picture18.png)

## Screen Recording
The following link shows a screen recording of the project in action. The screencast demonstrates:
* Working deployed ML model endpoint
* Deployed Pipeline
* Available AutoML Model
* Successful API requests to the endpoint with a JSON payload
https://www.youtube.com/watch?v=MrXGluUcm9c&ab_channel=N%C3%ADcolasWeisdeSouzaPauli

## Future improvements
Different techniques can be used to improve the model performance among them include feature engineering, feature selection, ensemble methods, algorithm tunning and cross-validation. In this dataset case, more samples could be added to improve the learning process of the algorithm to retain more patterns. The dataset presented class imbalance, solving this problem would result in a better accuracy. The training time was also limited, so with more training time the model could capture other different patterns. 
