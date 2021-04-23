## Add machine learning to search relevance - Azure Search + Azure ML

This tutorial demonstrates how to call search service api to Azure Search and register a model in Azure Machine Learning and create Azure Container Instance in Azure Machine Learning. As such this tutorial is targerted to developers who wants to improve their search relevance using Azure Search Relevance and create a machine learning model to improve the ranking of search outputs. 

The architecture that can be proposed is as follow:
<img width="2427" alt="image" src="https://user-images.githubusercontent.com/82999408/115831650-773ab680-a444-11eb-9d3f-bbd417c590cb.png">

In this tutorial, we would upload our dataset into Azure Blob Storage and choose this dataset directory when we create our Azure Search Service. There is a lot of choices of the dataset type and dataset location. It can be in Azure Blob Storage, Azure Cosmos DB, Azure SQL Database or Azure SQL Datawarehouse. After placing our dataset and running a model, we would need to register our model in Azure Machine Learning and deploy our model in Azure Container Instance. After deploying the model in Azure Container Instance, our web user interface can call the api to the Container Instance to retrieve the results from our model when someone enters a query in the user interface.
