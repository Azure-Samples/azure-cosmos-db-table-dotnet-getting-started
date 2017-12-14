# Getting started with Azure Cosmos DB Table API
[Azure Cosmos DB](http://cosmosdb.com) is a globally distributed, multi-model database for mission critical applications. 
Azure Cosmos DB provides the [Table API](https://docs.microsoft.com/azure/cosmosdb/table-introduction.md) for users of
Azure Table storage who need more premium features. 

## About this sample: CRUD and Query using the Azure Table storage preview SDK

Azure Cosmos DB supports the Table API using a number of SDKs including the .NET SDK that is demonstrated in this sample. 
You can download the [Azure Cosmos DB Table API SDK from Nuget](https://www.nuget.org/packages/Microsoft.Azure.CosmosDB.Table), this is now the official
SDK both for Azure Cosmos DB Table API as well as for Azure Table storage.

This sample is for developers who are familiar with the Azure Table storage SDK, and would like to use the premium features available using Azure Cosmos DB Table API. 
It is based on Get Started with Azure Table storage using .NET and shows how to take advantage of additional capabilities like secondary indexes, provisioned throughput, and multi-homing. 

* Open in Visual Studio
* Update the connection string in App.config to your Azure Cosmos DB Table API account endpoint and keys, e.g. `<add key="CosmosDBStorageConnectionString" value="DefaultEndpointsProtocol=https;AccountName=account-name;AccountKey=account-key;TableEndpoint=https://account-name.table.cosmosdb.azure.com;" />`
* Run the application

If you would like to try this sample with Azure Table storage then set the key StandardStorageConnectionString to your Azure storage account connection string in App.config and 
specify the argument "Standard" on the command line when you run the sample.

## Azure Cosmos DB Table API overview
If you currently use Azure Table storage, you gain the following benefits with the preview:

* Turn-key global distribution with multi-homing and automatic and manual failvoers
* Support for automatic schema-agnostic indexing against all properties ("secondary indexes"), and fast queries
* Support for independent scaling of storage and throughput, across any number of regions
* Support for dedicated throughput per table that can be scaled from 100s to millions of requests per second
* Support for five tunable consistency levels to trade off availability, latency, and consistency based on your application needs
* 99.99% availability within a single region, and ability to add more regions for higher availability, and industry-leading comprehensive SLAs on general availability
* Work with the existing Azure storage .NET SDK, and no code changes to your application

For more information please see the [Introduction to Azure Cosmos DB Table API](https://docs.microsoft.com/en-us/azure/cosmos-db/table-introduction).