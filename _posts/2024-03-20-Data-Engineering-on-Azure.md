---
layout: post
title: Data Engineering with Azure
subtitle: Learning data engineering with azure
categories: Data Engineering
tags: [Azure, Data Engineering, certificate]
---

## Introduction to data engineering on Azure
1. What is data engineering:
   
   Data engineering is the process of integrating, transforming, and consolidating data from various structured and unstructured data systems into structures that are suitable for building analytics solutions.

2. Important data engineering concepts

   There are some concepts that data engineers should be familiar. which are:

   i. Operational and analytical data

   ii. Streaming data

   iii. Data pipelines

   iv. Datalakes

   v. Data warehouses

   vi. Apache Spark

3. Data engineering in Microsoft Azure
   Data engineers using Azure for ETL should be familiar with the following tools:
   Azure Stream Analytics,
   Azure Data Factory,
   Azure Databricks,
   Azure Synapse Analytics,
   Azure Data Lake Storage Gen2,

## Use Azure Synapse serverless SQL pool to query files in a data lake 
1. Understand Azure Synapse serverless SQL pool capabilities and use cases:
   Synapse serverless SQL pool is used by data engineers the query data in datalake gen2 container.

2. Query files using a serverless SQL pool:
   The types of file that are been queried in serverless SQL pool are:
   parquet file,
   CSV file,
   JSON file

## Analyze data with Apache Spark in Azure Synapse Analytics 
1. What is Apache Spark:

   Apache Spark is an open source processing framework for large-scale data processing and analytics.

2. Use Spark in Azure Synapse Analytics:

   You can run many different kinds of application on Spark, including code in Python or Scala scripts, Java code compiled as a Java Archive (JAR), and others. Spark is commonly used in two kinds of workload.

3. Analyze data with Spark:
   
   One of the benefits of using Spark is that you can write and run code in various programming languages, enabling you to use the   programming skills you already have and to use the most appropriate language for a given task.

4. Visualize data with Spark:
   
   One of the most intuitive ways to analyze the results of data queries is to visualize them as charts. Notebooks in Azure Synapse Analytics provide some basic charting capabilities in the user interface, and when that functionality doesn't provide what you need, you can use one of the many Python graphics libraries to create and display data visualizations in the notebook.

## Analyze data in a relational data warehouse 
1. Design a data warehouse schema:
   
   Like all relational databases, a data warehouse contains tables in which the data you want to analyze is stored.

   Tables in a data warehouse.
   
   A common pattern for relational data warehouses is to define a schema that includes two kinds of table: dimension tables and fact tables.

   Dimension tables: 
   Dimension tables describe business entities, such as products, people, places, and dates. Dimension tables contain columns for attributes of an entity.

   Fact tables: 
   Fact tables store details of observations or events; for example, sales orders, stock balances, exchange rates, or recorded temperatures.

## Create data warehouse tables
1. Creating a dedicated SQL pool:
   
   To create a relational data warehouse in Azure Synapse Analytics, you must create a dedicated SQL Pool. The simplest way to do this in an existing Azure Synapse Analytics workspace is to use the Manage page in Azure Synapse Studio.

3. Load data warehouse tables:
   
   As a data engineer you can load data into your data warehouse from any data source, either from your your datalake or the web.

5. Query a data warehouse:
   
   When the dimension and fact tables in a data warehouse have been loaded with data, you can use SQL to query the tables and analyze the data they contain. The Transact-SQL syntax used to query tables in a Synapse dedicated SQL pool is similar to SQL used in SQL Server or Azure SQL Database.

## Build a data pipeline in Azure Synapse Analytics   
1. Understand pipelines in Azure Synapse Analytics:
   Pipelines in Azure Synapse Analytics encapsulate a sequence of activities that perform data movement and processing tasks. You can use a pipeline to define data transfer and transformation activities, and orchestrate these activities through control flow activities that manage branching, looping, and other typical processing logic. The graphical design tools in Azure Synapse Studio enable you to build complex pipelines with minimal or no coding required.

2. Create a pipeline in Azure Synapse Studio:
   You can create a pipeline in Azure Synapse Studio by using shortcuts on the Home page, but the primary place where pipelines are created and managed is the Integrate page.

3. Define data flows:
   A Data Flow is a commonly used activity type to define data flow and transformation. Data flows consist of:

   Sources - The input data to be transferred.
  
   Transformations – Various operations that you can apply to data as it streams through the data flow.
  
   Sinks – Targets into which the data will be loaded.

4. Run a pipeline:
  When you’re ready, you can publish a pipeline and use a trigger to run it. Triggers can be defined to run the pipeline:

  i. Immediately
  
  ii. At explicitly scheduled intervals
  
  iii. In response to an event, such as new data files being added to a folder in a data lake.

## Data engineering with Azure Databricks
  ### Explore Azure Databricks
  1. Get started with Azure Databricks
     Azure Databricks is a cloud-based distributed platform for data processing and analytics in a data lakehouse. Databricks is built on Apache Spark and related open source technologies, and is designed to unify data science, data engineering, and business data analytics in an easy to use environment that enables users to spend more time working effectively with data, and less time focused on managing clusters and infrastructure.

  2. Identify Azure Databricks workloads
     Azure Databricks is a comprehensive platform that offers many data processing capabilities. While you can use the service to support any workload that requires scalable data processing, Azure Databricks particularly supports the following types of data workload:

     Data Science and Engineering

     Machine Learning

     SQL

  3. Understand key concepts
     Azure Databricks is an amalgamation of multiple technologies that enable you to work with data at scale. Before using Azure Databricks, there are some key concepts that you should understand.
     i. Apache Spark clusters - Spark is a distributed data processing solution that makes use of clusters to scale processing across multiple compute nodes.

     ii. Data lake storage - While each cluster node has its own local file system (on which operating system and other node-specific files are stored), the nodes in a cluster also have access to a shared, distributed file system in which they can access and operate on data files.
  
     iii. Metastore - Azure Databricks uses a metastore to define a relational schema of tables over file-based data. The tables are based on the Delta Lake format and can be queried using SQL syntax to access the data in the underlying files.
  
     iv. Notebooks - One of the most common ways for data analysts, data scientists, data engineers, and developers to work with Spark is to write code in notebooks.
  
     v. SQL Warehouses - SQL Warehouses are relational compute resources with endpoints that enable client applications to connect to an Azure Databricks workspace and use SQL to work with data in tables. The results of SQL queries can be used to create data visualizations and dashboards to support business analytics and decision making.
  
  ### Use Apache Spark in Azure Databricks
  1. Get to know Spark
     To gain a better understanding of how to process and analyze data with Apache Spark in Azure Databricks, it's important to understand the underlying architecture.

  2. Create a Spark cluster:
     When creating the cluster, you can specify configuration settings, including:

     i. A name for the cluster.

     ii. A cluster mode, which can be:

         a. Standard: Suitable for single-user workloads that require multiple worker nodes.

         b. High Concurrency: Suitable for workloads where multiple users will be using the cluster concurrently.

         c. Single Node: Suitable for small workloads or testing, where only a single worker node is required.

     iii. The version of the Databricks Runtime to be used in the cluster; which dictates the version of Spark and individual components such as Python, Scala, and others that get installed.

     iv. The type of virtual machine (VM) used for the worker nodes in the cluster.

     v. The minimum and maximum number of worker nodes in the cluster.

     vi. The type of VM used for the driver node in the cluster.

     vii. Whether the cluster supports autoscaling to dynamically resize the cluster.

     viii. How long the cluster can remain idle before being shut down automatically.

  3. Use Spark in notebooks:
     ou can run many different kinds of application on Spark, including code in Python or Scala scripts, Java code compiled as a Java Archive (JAR), and others. Spark is commonly used in two kinds of workload:

    i.  Batch or stream processing jobs to ingest, clean, and transform data - often running as part of an automated pipeline.
    ii. Interactive analytics sessions to explore, analyze, and visualize data.

  4. Use Spark to work with data files:
     One of the benefits of using Spark is that you can write and run code in various programming languages, enabling you to use the programming skills you already have and to use the most appropriate language for a given task.
     
  5. Visualize data:
     One of the most intuitive ways to analyze the results of data queries is to visualize them as charts. Notebooks in Azure Databricks provide charting capabilities in the user interface, and when that functionality doesn't provide what you need, you can use one of the many Python graphics libraries to create and display data visualizations in the notebook.

  ### Use Delta Lake in Azure Databricks
  1. Get Started with Delta Lake
     Delta Lake is an open-source storage layer that adds relational database semantics to Spark-based data lake processing. Delta Lake is supported in Azure Synapse Analytics Spark pools for PySpark, Scala, and .NET code.

  2. Create Delta Lake tables
     One of the easiest ways to create a Delta Lake table is to save a dataframe in the delta format, specifying a path where the data files and related metadata information for the table should be stored.

  3. Create and query catalog tables:
     So far we've considered Delta Lake table instances created from dataframes and modified through the Delta Lake API. You can also define Delta Lake tables as catalog tables in the metastore and work with them using SQL.

  4. Use Delta Lake for streaming data:
     All of the data we've explored up to this point has been static data in files. However, many data analytics scenarios involve streaming data that must be processed in near real time.

  ### Use SQL Warehouses in Azure Databricks
  1. Get started with SQL Warehouses:
     SQL Warehouses (formerly known as SQL Endpoints) provide a relational database interface for data in Azure Databricks. The data is stored in files that are abstracted by Delta tables, but from the perspective of the user or client application, the SQL Warehouse behaves like a relational database.

  2. Create databases and tables:
     After creating and starting a SQL Warehouse, you can start to work with data in tables.

     i. Database schema:
       All SQL Warehouses contain a default database schema named default. You can use create tables in this schema in order to analyze data

     ii. Tables
       You can use the user interface in the Azure Databricks portal to upload delimited data, or import data from a wide range of common data sources.
  
  3. Create queries and dashboards:
     Azure Databricks SQL is primarily designed for data analytics and visualization workloads. To support these workloads, users can create queries to retrieve and summarize data from tables, and dashboards to share visualizations of the data.

  ### Run Azure Databricks Notebooks with Azure Data Factory
  1. Understand Azure Databricks notebooks and pipelines:
     In Azure Databricks, you can use notebooks to run code written in Python, Scala, SQL, and other languages to ingest and process data. Notebooks provide an interactive interface in which you can run individual code cells and use Markdown to include notes and annotations.

  2. Create a linked service for Azure Databricks:
     To run notebooks in an Azure Databricks workspace, the Azure Data Factory pipeline must be able to connect to the workspace; which requires authentication. To enable this authenticated connection, you must perform two configuration tasks:

      i. Generate an access token for your Azure Databricks workspace.
      ii. Create a linked service in your Azure Data Factory resource that uses the access token to connect to Azure Databricks.
    
   3. Use a Notebook activity in a pipeline:
      After you've created a linked service in Azure Data Factory for your Azure Databricks workspace, you can use it to define the connection for a Notebook activity in a pipeline.

   4. Use parameters in a notebook
      You can use parameters to pass variable values to a notebook from the pipeline. Parameterization enables greater flexibility than using hard-coded values in the notebook code.
