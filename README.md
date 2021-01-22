# Operarionalizing Machine Learning in Azure

This project aims to demonstrate how to train a model using Azure Machine Learning Studio and put it in production to an end user. The dataset used was Banking Marketing dataset, where the goal is to predict whether a client would sign a bank term deposit based on several features. The training process was made entirely using Auto ML through Azure Machine Learning Studio. After that, it was chosen the best model to accordingly with the best algorithm, VotingEnsemble and deployed into production. With the deployed model, it was enabled the Application Insight using Azure Python SDK. For the documentation, it was used Swagger instance running with the documentation for the HTTP API of the model. The model was consumed using the deployed scoring URI and key authentication running the endpoint.py script against the API producing JSON output from the model. I was used Apache Benchmark to retrieve the performance result details running against the HTTP API. Finally, it was created, deployed and consumed a pipeline. The model and the pipeline can be accessed through REST terminals.

## Architectural Diagram


The following steps were performed in order to complete this project:
Authentication
Automated ML Experiment
Deploy the best model
Enable logging
Swagger Documentation
Consume model endpoints
Create and publish a pipeline
Documentation

## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screenshots required to demonstrate key steps. 

## Screen Recording
The following link shows a screen recording of the project in action. The screencast demonstrates:
Working deployed ML model endpoint
Deployed Pipeline
Available AutoML Model
Successful API requests to the endpoint with a JSON payload
https://www.youtube.com/watch?v=MrXGluUcm9c&ab_channel=N%C3%ADcolasWeisdeSouzaPauli

## Future improvements
Different techniques can be used to improve the model performance among them feature engineering, feature selection, ensemble methods, algorithm tunning and cross-validation. In this dataset case, more samples could be added to improve the learning process of the algorithm to retain more patterns. The dataset presented class imbalance, solving this problem would result in a better accuracy. The training time was also limited, so with more training time the model could capture other different patterns. 
