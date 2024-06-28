---
layout: post
title: Using Power Bi for Data Analytics
subtitle: Learning how to Use Power BI for Analytics Purpose
categories: Python
tags: [Power BI, Data Analytics, intro, certificate]
---

# Power BI with Data Analytics
## Get started with Microsoft data analytics
1. Introduction

As a data analyst, you are on a journey. Think about all the data that is being generated each day and that is available in an organization, from transactional data in a traditional database, telemetry data from services that you use, to signals that you get from different areas like social media.

2. Overview of data analysis

Before data can be used to tell a story, it must be run through a process that makes it usable in the story. Data analysis is the process of identifying, cleaning, transforming, and modeling data to discover meaningful and useful information. The data is then crafted into a story through reports for analysis to support the critical decision-making process.

While the process of data analysis focuses on the tasks of cleaning, modeling, and visualizing data, the concept of data analysis and its importance to business should not be understated. To analyze data, core components of analytics are divided into the following categories:

i. Descriptive

ii. Diagnostic

iii. Predictive

iv. Prescriptive

v. Cognitive

3. Roles in data

Telling a story with the data is a journey that usually doesn't start with you. The data must come from somewhere. Getting that data into a place that is usable by you takes effort that is likely out of your scope, especially in consideration of the enterprise.

4. Tasks of a data analyst

A data analyst is one of several critical roles in an organization, who help uncover and make sense of information to keep the company balanced and operating efficiently. Therefore, it's vital that a data analyst clearly understands their responsibilities and the tasks that are performed on a near-daily basis. Data analysts are essential in helping organizations gain valuable insights into the expanse of data that they have, and they work closely with others in the organization to help reveal valuable information.

## Prepare data for analysis with Power BI
1. Get data from files

Organizations often export and store data in files. One possible file format is a flat file. A flat file is a type of file that has only one data table and every row of data is in the same structure. The file doesn't contain hierarchies. Likely, you're familiar with the most common types of flat files, which are comma-separated values (.csv) files, delimited text (.txt) files, and fixed width files. Another type of file would be the output files from different applications, like Microsoft Excel workbooks (.xlsx).

2. Get data from relational data sources

If your organization uses a relational database for sales, you can use Power BI Desktop to connect directly to the database instead of using exported flat files.

Connecting Power BI to your database will help you to monitor the progress of your business and identify trends, so you can forecast sales figures, plan budgets and set performance indicators and targets. Power BI Desktop can connect to many relational databases that are either in the cloud or on-premises.

3. Create dynamic reports with parameters

Dynamic reports are reports in which the data can be changed by a developer according to user specifications. Dynamic reports are valuable because a single report can be used for multiple purposes. If you use dynamic reports, you'll have fewer individual reports to create, which will save organizational time and resources.

4. Get data from a NoSQL database

Some organizations don't use a relational database but instead use a NoSQL database. A NoSQL database (also referred to as non-SQL, not only SQL or non-relational) is a flexible type of database that doesn't use tables to store data.

5. Select a storage mode

The most popular way to use data in Power BI is to import it into a Power BI semantic model. Importing the data means that the data is stored in the Power BI file and gets published along with the Power BI reports. This process helps make it easier for you to interact directly with your data. However, this approach might not work for all organizations.

6. Get data from Azure Analysis Services

Azure Analysis Services is a fully managed platform as a service (PaaS) that provides enterprise-grade semantic models in the cloud. You can use advanced mashup and modeling features to combine data from multiple data sources, define metrics, and secure your data in a single, trusted tabular semantic model. The semantic model provides an easier and faster way for users to perform ad hoc data analysis using tools like Power BI.

7. Fix performance issues

Occasionally, organizations will need to address performance issues when running reports. Power BI provides the Performance Analyzer tool to help fix problems and streamline the process.

8. Resolve data import errors
Completed
100 XP
7 minutes
While importing data into Power BI, you may encounter errors resulting from factors such as:

i Power BI imports from numerous data sources.

ii. Each data source might have dozens (and sometimes hundreds) of different error messages.

iii. Other components can cause errors, such as hard drives, networks, software services, and operating systems.

iv Data often can't comply with any specific schema.

## Model data with Power BI
1. Introduction

In Microsoft Power BI, the semantic model underpins report and dashboard development. To produce the right reports and dashboards, you should have a clear understanding of the questions that your report and dashboard users will ask. Your next focus should be on the semantic model design that will best support the visualizations in your reports and dashboards. After you've arrived at a model design, you're ready to use Power BI Desktop to develop the model.

2. Star schema design

It's unusual for a Power BI semantic model to be comprised of a single table. A single-table model can be a simple design, perhaps one that's suitable for a data exploration task or proof of concept, but not one that's an optimal model design. An optimal model adheres to star schema design principles. Star schema refers to a design approach that's commonly used by relational data warehouse designers because it presents a user-friendly structure and it supports high-performance analytic queries.

3. Analytic queries
Completed
100 XP
2 minutes
An analytic query is a query that produces a result from a semantic model. Each Power BI visual, in the background, submits an analytic query to Power BI to query the model. The analytic query is written as a Data Analysis Expressions (DAX) query statement. However, you don't need to write a native DAX statement; you only need to configure report visuals by mapping semantic model fields.

An analytic query has three phases that are implemented in the following order:

Filter

Group

Summarize

3. Configure report visuals

Report authors produce report designs by adding report visuals and other elements to pages. Other elements include text boxes, buttons, shapes, and images. Each of these elements is configured independently of semantic model fields.

At design time, adding and configuring a report visual involves the following methodology:

i. Select a visual type, like a bar chart.

ii. Map semantic model fields, which are displayed in the Fields pane, to the visual field wells. For a bar chart, the wells are Y-axis, X-axis, Legend, Small multiples, and Tooltips.

iii Configure mapped fields. It's possible to rename mapped fields or toggle the field to summarize or not summarize. If the field summarizes, you can select the summarization method.

iv. Apply format options, like axis properties, data labels, and many others.

## Build Power BI visuals and reports
1. Introduction

As with any project, a good starting point when designing reports is to define clear goals. In your reporting project, those goals should strive to help you determine your reporting requirements for:

Audiences

Report type

User interface requirements

User experience requirements

2. Identify the audience

Identifying the audience is one of the most important steps in the report design process. It enables the report author to create a final result that can be efficiently used and will meet the needs of the report consumer.

The three broad report consumer audiences are:

Executive

Analyst

Information worker

3. Determine report types

Generally, report design can be classified by report type. Often, a direct mapping between the report audience and the report type occurs. Audience needs can be met by one, or possibly a combination, of four report types:

Dashboard

Analytical

Operational

Educational

4. Define user experience requirements

UX requirements relate to how reports deliver the expected report consumer needs. To assess user experience requirements, you should consider the audience, report type, and the UI requirements.

## Manage workspaces and datasets in Power BI
1. Distribute a report or dashboard

Consider a scenario where you have created a few reports for the Sales team at Tailwind Traders. The issue that you have encountered is determining how to make these reports viewable and shareable. By creating a workspace in Power BI, you can house your reports in one location, make them shareable, collaborate with other teams, and update reports.

2. Monitor usage and performance

Knowing about the usage and performance of your workspace is crucial because it:

i. Focuses your efforts for improvement. If you know the areas that experience the worst performance, you can concentrate your efforts for improvement in those areas.

ii. Quantifies the impact of your reports. Usage metrics help you determine your reports' success.

3. Recommend a development life cycle strategy

The development process is iterative; it typically requires building an initial solution, testing the solution in a different environment, returning to make necessary revisions, and eventually releasing a final product. This process is known as a development life cycle. This process can take place in several different ways and in different environments.

4. Configure data protection

As enterprises grow, so does their data. Often, strict requirements and regulations must be applied to ensure that this sensitive data is secure. Power BI provides a few different ways to help you accomplish this task:

i. Use Microsoft sensitivity labels to label dashboards, reports, semantic models, and dataflows by using the same taxonomy that is used to classify and protect files in Microsoft 365.

ii. Add more protection measures such as encryption and watermarks when you are exporting the data.

iii. Use Microsoft Cloud App Security to monitor and investigate activities in Power BI.
