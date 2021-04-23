## Add machine learning to search relevance - Azure Search + Azure ML

This tutorial demonstrates how to call search service api to Azure Search and register a model in Azure Machine Learning and create Azure Container Instance in Azure Machine Learning. As such this tutorial is targerted to developers who wants to improve their search relevance using Azure Search Relevance and create a machine learning model to improve the ranking of search outputs. Please make sure you have an Azure Account created if you would like to follow through the whole tutorial. 

In this tutorial, we would upload our dataset into Azure Blob Storage and choose this dataset directory when we create our Azure Search Service. There is a lot of choices of the dataset type and dataset location. It can be in Azure Blob Storage, Azure Cosmos DB, Azure SQL Database or Azure SQL Datawarehouse. After placing our dataset and running a model, we would need to register our model in Azure Machine Learning and deploy our model in Azure Container Instance. After deploying the model in Azure Container Instance, our web user interface can call the api to the Container Instance to retrieve the results from our model when someone enters a query in the user interface.

## Getting Started

If you only want to read the code, u can focus on 

Part 1: [predict-link-xgboost-part1-github.ipynb](https://github.com/siaodevil/azure-search-and-ml/blob/main/predict-link-xgboost-part1-github.ipynb) to understand how to call azure search api and register a model in Azure Machine Learning

Part 2: predict-link-xgboost-part2-github.ipynb to understand create a image of the model in Azure Containter Instance using Azure Machine Learning

Part 3: predict-link-automl-github.ipynb to understand how to call automated ML using code instead of the interface available in Azure Machine Learning

To follow through this whole tutorial, you can start of with 
1. PDF: Guide for Azure Search Service
2. PDF: Guide for Azure Machine Learning
3. Code: predict-link-xgboost-part1-github.ipynb 
4. Code: predict-link-xgboost-part2-github.ipynb 
5. Code: predict-link-automl-github.ipynb (optional)

## Requirements to follow the tutorial

1. Azure Account created
2. Azure Search Service created
3. Azure Blob Storage created
4. Azure Machine Learning created

The architecture of this whole tutorial is as follow:

<img width="666" alt="image" src="https://github.com/siaodevil/azure-search-and-ml/blob/main/architecture.png">

