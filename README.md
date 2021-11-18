> **<span class="underline">Prerequisite:</span>**
>
> Participants should know Docker and Kubernetes and Cloud Computing
> concepts
>
> Participants need to read the material and do exercises provided by
> trainer daily after session is over


**<span class="underline">Installation, Administration and Configuration</span>**

1.  The basics of Apache Airflow

    -  What is Airflow?

    -  How does Airflow work?

    -  Overview of Airflow UI

    -  Overview of Airflow CLI

1.  Airflow Installation

    -  Using Production Docker Images

    -  Using Official Airflow Helm Chart

    -  Using Managed Airflow Services

    -  Using 3rd-party images, charts, deployments

1.  Add tags to DAGs and use it for filtering in the UI

1.  Setting Configuration Options

1.  Set up a Database Backend

    -  Choosing database backend

    -  Database URI

    -  Setting up a SQLite Database

    -  Setting up a MySQL Database

    -  Setting up a PostgreSQL Database

    -  Initialize the database

1.  Using Operators

    -  BashOperator

        -  Templating

        -  Skipping

        -  Troubleshooting

    -  BranchDateTimeOperator

    -  PythonOperator

        -  Passing in arguments

        -  Templating

    -  PythonVirtualenvOperator

        -  Passing in arguments

        -  Templating

    -  BranchDayOfWeekOperator

    -  Cross-DAG Dependencies

        -  ExternalTaskSensor

        -  ExternalTaskMarker

**<span class="underline">Configuration and Development</span>**

1.  Creating a custom Operator

    -  Hooks

    -  User interface

    -  Templating

    -  Define an operator extra link

    -  Sensors

1.  Managing Connections

    -  Creating a Connection with the UI

    -  Editing a Connection with the UI

    -  Creating a Connection from the CLI

    -  Exporting Connections from the CLI

    -  Storing a Connection in Environment Variables

    -  Connection URI format

    -  Securing Connections

    -  Custom connection types

1.  Managing Variables

    -  Storing Variables in Environment Variables

    -  Securing Variables

1. Using the Test Mode Configuration

1. The Forex Data Pipeline

    -  Introduction

    -  What is a DAG?

    -  Defining first DAG

    -  What is an Operator?

    -  Checking if the API is available - HttpSensor

    -  Checking if the currency file is available - FileSensor

    -  Downloading the forex rates from the API - PythonOperator

    -  Saving the forex rates in the HDFS - BashOperator

    -  Creating the Hive table forex\_rates - HiveOperator

    - Processing the forex rates with Spark - SparkSubmitOperator

    - Sending an email notification - EmailOperator

    - Sending a Slack notification - SlackAPIPostOperator

    - Operator Relationships and Bitshift Composition

    - Adding dependencies between tasks

    - The Forex Data Pipeline in action\!

**<span class="underline">Configuration and Development</span>**

1. Mastering DAGs

    -  Introduction

    -  Start\_date and schedule\_interval parameters

    -  Manipulating the start\_date with schedule\_interval

    -  Backfill and Catchup

    -  Catching up non triggered DAGRuns

    -  Dealing with timezones in Airflow

    -  Making DAGs timezone aware

    -  How to make tasks dependent?

    -  Creating task dependencies between DagRuns

    - How to structure a DAG folder?

    - Organizing DAGs folder

    - How does the Web Server work?

    - How to deal with failures in DAGs?

    - Retry and Alerting

    - How to test DAGs?

    - Unit testing DAGs

1. Distributing Apache Airflow

    -  Introduction

    -  Sequential Executor with SQLite

    -  Local Executor with PostgreSQL

    -  Executing tasks in parallel with the Local Executor

    -  Ad Hoc Queries with the metadata database

    -  Scale out Apache Airflow with Celery Executors and Redis

    -  Set up the Airflow cluster with Celery Executors and Docker

    -  Distributing tasks with the Celery Executor

    -  Adding new worker nodes with the Celery Executor

    - Sending tasks to a specific worker with Queues

    - Pools and priority\_weights: Limiting parallelism -
        prioritizing tasks

    - Kubernetes Overview

    - Scaling Airflow with Kubernetes Executors

    - Installing Airflow with Rancher and the Kubernetes Executor

    - Running DAGs with the Kubernetes Executor

**<span class="underline">Configuration and Development</span>**

1. Improving DAGs with advanced concepts

    -  Introduction

    -  Minimising Repetitive Patterns With SubDAGs

    -  Grouping tasks with SubDAGs and Deadlocks

    -  Making different paths in DAGs with Branching

    -  Make First Conditional Task Using Branching

    -  Trigger rules for tasks

    -  Changing how tasks are triggered

    -  Avoid hard coding values with Variables, Macros and Templates

    -  Templating tasks

    - How to share data between tasks with XCOMs?

    - Sharing (big?) data with XCOMs

    - Trigger DagRunOperator or when DAG controls another DAG

    - Trigger a DAG from another DAG

    - Dependencies between DAGs with the ExternalTaskSensor

    - Make DAGs dependent with the ExternalTaskSensor

1. Deploying Airflow with Kubernetes Executors and Rancher

    -  Introduction

    -  Quick overview of EKS

    -  Set up an EC2 instance for Rancher

    -  Create an IAM User with permissions

    -  Create an ECR repository

    -  Create an EKS cluster with Rancher

    -  How to access applications from the outside?

    -  Deploy Nginx Ingress with Catalogs (Helm)

    -  Deploy and run Airflow with the Kubernetes Executor on EKS

**<span class="underline">Configuration and Development</span>**

1. Monitoring Apache Airflow

    -  Introduction

    -  How does the logging system work in Airflow?

    -  Setting up custom logging

    -  Storing logs in Azure

    -  Elasticsearch Overview

    -  Configuring Airflow with Elasticsearch

    -  Monitoring your DAGs with Elasticsearch

    -  Introduction to metrics

    -  Monitoring Airflow with TIG stack

    - Triggering alerts for Airflow with Grafana

    - Airflow maintenance DAGs

1. Security in Apache Airflow

    -  Introduction

    -  Encrypting sensitive data with Fernet

    -  Rotating the Fernet Key

    -  Hiding variables

    -  Password authentication and filter by owner

    -  RBAC UI

1. Ways to deploy Airflow on AWS

    -  Deploy airflow on AWS EKS

    -  Deploy airflow on AWS EC2

    -  Use the managed airflow service on AWS

        -  Create an environment

        -  Upload your DAGs and plugins to S3

        -  Run your DAGs in Airflow
