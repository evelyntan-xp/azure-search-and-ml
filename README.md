## Add machine learning to search relevance - Azure Search + Azure ML

This tutorial demonstrates how to call search service api to Azure Search and register a model in Azure Machine Learning and create Azure Container Instance in Azure Machine Learning. As such this tutorial is targerted to developers who wants to improve their search relevance using Azure Search Relevance and create a machine learning model to improve the ranking of search outputs. Please make sure you have an Azure Account created if you would like to follow through the whole tutorial. 

In this tutorial, we would upload our dataset into Azure Blob Storage and choose this dataset directory when we create our Azure Search Service. There is a lot of choices of the dataset type and dataset location. It can be in Azure Blob Storage, Azure Cosmos DB, Azure SQL Database or Azure SQL Datawarehouse. After placing our dataset and running a model, we would need to register our model in Azure Machine Learning and deploy our model in Azure Container Instance. After deploying the model in Azure Container Instance, our web user interface can call the api to the Container Instance to retrieve the results from our model when someone enters a query in the user interface.

## Getting Started

If you only want to read the code, u can focus on 

Part 1: [predict-link-xgboost-part1-github.ipynb](https://github.com/siaodevil/azure-search-and-ml/blob/main/predict-link-xgboost-part1-github.ipynb) to understand how to call azure search api and register a model in Azure Machine Learning

Part 2: [predict-link-xgboost-part2-github.ipynb](https://github.com/siaodevil/azure-search-and-ml/blob/main/predict-link-xgboost-part2-github.ipynb) to understand create a image of the model in Azure Containter Instance using Azure Machine Learning

Part 3: [predict-link-automl-github.ipynb](https://github.com/siaodevil/azure-search-and-ml/blob/main/predict-link-automl-github.ipynb) to understand how to call automated ML using code instead of the interface available in Azure Machine Learning

To follow through this whole tutorial, you can start off with 
1. PDF: [Guide for Azure Search Service](https://github.com/siaodevil/azure-search-and-ml/blob/main/Guide%20for%20Azure%20Search%20Service.pdf)
  2. -- Update the api_config.json file followingly
3. PDF: [Guide for Azure Machine Learning](https://github.com/siaodevil/azure-search-and-ml/blob/main/Guide%20for%20Azure%20Machine%20Learning.pdf)
4. Code: predict-link-xgboost-part1-github.ipynb 
5. Code: predict-link-xgboost-part2-github.ipynb 
6. Code: predict-link-automl-github.ipynb (optional)

## Requirements to follow the tutorial

1. Azure Account created --> you can follow leekokhow github Page 1 to 15 of [Quickstart Guide for Using Azure Machine Learning](https://github.com/leekokhow/azureml/blob/master/Quickstart%20Guide%20for%20Using%20Azure%20Machine%20Learning.pdf) to understand how to create an Azure Account and Azure Machine Learning Service. 
2. Azure Blob Storage created
3. Azure Search Service created --> follow PDF: Guide for Azure Search Service
4. Azure Machine Learning created 

The architecture of this whole tutorial is as follow:

<img width="666" alt="image" src="https://github.com/siaodevil/azure-search-and-ml/blob/main/architecture.png">


### Acknowledgement
I would like to thank LeeKokHow github code to kickstart my learning into Azure Machine Learning. 
