# Introduction to Snowflake
i) Cloud Oriented
ii) Data Platform
iii)SaaS

i) Cloud Oriented
  -Snowflake's software purposely built for Cloud.
  -Makes use of elasticity, scalability, high availabilty, cost-efficiency & durability.

ii)  Data Platform
   -1. Data Warehouse:
	1.1 Structured & relational data
	1.2 ANSI Standard SQL
	1.3 ACID complaiant transactiobs
	1.4 Data stored in databases,schemas & tables
   -2. Data Lake
	2.1 Scalable storage and compute
	2.2 Schema does not need to be defined upfront
	2.3 Native processing of semi-structured data formats
   -3. Data Engineering
	3.1 COPY INTO & Snowpipe
	3.2 Seperate compute clusters
	3.3 Tasks and Streams
	3.4 All data encrypted at rest and in transit
   -4. Data Science
	4.1 Remove data management roadblocks with centralised storage
	4.2 Partner ecosystem includes data science tooling like Amazon Sagemaker, DataRobot, Dataiku
   -5. Data Sharing
	5.1 Secure Data Sharing 
	5.2 Data Exchange 
	5.3 BI with Snowflake partner ecosystem tools. 
   -6. Data Applications
	6.1 Connectors and Drivers
	6.2 UDFs and Stored Proceders
	6.3 External UDFs
	6.4 Preview feauters such as Snowpark

iii) SaaS
	- No management of hardware
	- Transparent system updates and patches
	- Subscription payment
	- Ease of access
	- Automatic optimisation

# Snowflake Architecture:
-The architecture is designed for scalability, performance and simplicity. Decouples storage, compute and management services.
- Key components: Storage layer(S3,GCS); Compute Layer (Virtual Warehouses); Services Layer

i) Storage Layer
-persistent and infinitely scalable cloud storage residing cloud providers e.g. AWS S3
-data loaded into Snowflake is organized by databases, schemas and tables.
-structred and semi structered data files can be loaded and stored in Snowflake.
-when data files are loaded, Snowflake reorganizes the data into proprietary, columnar table file format.
-data loaded is partionoed into micropartitions.
-storage billed by how much is stored based on a flat rate per TB monthly
-data not directly accessible in underlying blob storage only via SQL commands.	


ii) Compute Layer
-virtual warehouses executing processing tasks required to return results for SQL statements.
-virtual warehouse = named abstraction for cluster of cloud-based compute instances.
-nodes of VW cooperate same way to shared nothing compute clusters using local caching.
-VW can be created or removed instantly.
-paused or resumed
-ulimited no of VH can be created
-VH come in different sizes, relative compute power
-have consistant access to same data in storage layer

iii) Service Layer
-collection of highly available and scalable services coordinating servcies such as authentication and query optimization
-runs on cloud compute instances
-Services manages: authentication, infrastructure management, transaction management, metadata management, query optimisation and security




# Key Feautures & Capabilites 
-Seperation of Compute and Storage: unique architechture, decouples storage and compute resources. Users scale compute power up without affecting stored data
-Automatic Scaling: dynamically adjusts resources matched with demands, ensuring optimal performance without manual intervention.
-Multi-cluster Shared Data Architecture: allows multiple compute clusters to access same data simultaneously, enabling high concurreny without resource contention.
-Data Sharing: secure and controlled sharing of live data between Snowflake accounts & organizations, facilitating collaboration.
-Zero-Copy Cloning: provides ability to create instant, virtual copies of data without physical duplication. For dev, testin and analytics.
-Security and Governance: end-to-end encryption, granular access controls and comprehensive auditing capabilities for compliance with GDPR, HIPAA, etc.
-Support for Semi-Structured Data: supports semi-structured data like JSON, Avro, Parquet, etc. Versatile handling many data formats.
-Near-Zero Maintainace: handles maintanance tasks like patches, upgrades and backups,reducing operational burden on users.
-Query Perfomance Optimization: Snowflake's optimizer and query execution engine enhances query perfomance, leveraging indexing, partitioning and other optimization techniques.
-Elasticity and Cost Effeciency: pay-per-use pricing model, enables cost optimization techniques.
-Intergration and Ecosystem: intergrates seamlessly with various BI tools, data intergration platforms and programming languages, enabling easy data ingestion, transformation and analysis.
 


# Snowflake Editions and Cloud Platforms

## Snowflake Editions
-Standard: ideal for small to medium sized business or teams with basic data warehosing needs.
-Enteprise: designed for larger businesses requiring advanced features, greater scalability and enhanced security & governance.
-Business Critical: tailored for mission-critical workloads, offering additional features like higher service-level agreements(SLAs) and dedicated infrastructure.
-Virtual Private Snowflake: offers highest level of security for organizations like financial institutions and other large enterprises that collect, analyze and share sensitive data.
-includes all features and services of Business-Critical Edition but seperate Snowflake environment.


## Cloud Platforms
-AWS: snowflake operates on AWS utilizing infrastructure and services e.g. Amazon S3, EC2 and others.
-Azure: leverages blob storage, compute resources and other services.
-Google Cloud Platform (GCP): utilizes services like Google Cloud Storage and compute resources.




# Snowflake Data Loading and Unloading

## Data Loading Methods in Snowflake
i) Data Loading Tools: 
  -Snowflake Data Loading Wizard: a GUI within snowflake web interface to load data from various sources e.g. local files, Amazon S3. Azure Blob Storage and Google Cloud Storage
  -SnowSQL: command line tool provided by Snowflake allowing users to execute SQL commands, including loading data from diff sources.
  -Snowpipe: a continuous data ingestion service that automatically loads data into Snowflake tables from diff sources. Snowflake triggers table load whenever new data is detected.

ii) Bulk Loading:
   -Bulk Loading from Cloud Storage: supports loading data directly from cloud storage services using simple SQL commands('COPY INTO' statement).
   -Bulk Loading from On-Premises Storage: users can transfer large volumes of data securely from on-premises storage devices to Snowflake's cloud platform.

iii) ETL/ELT Tools:
    -intergrates with various Extract,Transform,Load(ETL) and Extract,Load,Transform(ELT) tools such as Talend, Informatica, Matillion, Fivetran etc. allowing users easily load data from diff sources.

iv) Other Methods:
	1) APIs: snowflake offers REST APIs enabling programmatic interactions, including loading data.
	2) Third-party Connectors: provide seamless intergration with many third-party applications and connectors.



## Data Unloading Methods in Snowflake
i) Data Unload Wizard:
   -provides a user-friendly web interface that allows users to unload data from Snowflake tables using a GUI.
   -users can select tables,specify file formats and define locations for unloading data.

ii) Unload Command
   -offers the 'COPY INTO' SQL command enabling users to export data from Snowflake tables into various file formats e.g. CSV,JSON,Parquet,Avro,ORC,etc.
   -the commmand exports data directly to cloud based storage or Snowflake internal stage locations.

iii) Command-Line Tool
    -SnowSQL allows users to execute SQL commands in a command-line environment.
    -method provides more control and flexibility for scripting and automating

## ETL/ELT Tools Intergrations

-various ETL/ETL tools intergrate with Snowflake can be used to unload data
-tools like Talend, Informatica, Matillion, Fivetran etc. provide functionalities to extract data from Snowflake to diff destinations.

Third Party Connectors/API

-Snowflake's REST APIs and 3rd party connectors may offer options to programmatically unload data to other locations.


# Data Transformation In Snowflake

## SQL for Data Transformation:
i) Standard SQL Operations:
-snowflake supports standard SQL operations(SELECT,INSERT,Update,Delete etc.) for manipulation.
-use these commands for filtering, aggregating, joining and transforming data.

ii) Built-in Functions:
-provides extensive built-in functions for string manipulation, math calculations, date and time operations, type conversions, etc.
-leverage functions like SUBSTRING,CONCAT,DATE_TRUNC,TO_DATE etc. for transformations.

iii) Windows Functions:
-utilize window functions like ROW_NUMBER,RANK,LEAD,LAG etc. for advanced queries and calculations over data sets.

## Views & Stored Procedures
i) Views:
-create views to encapsulate complex SQL queries and transformations.
-views can simplify data transformation processes by providing a logical layer over underlying data.

ii) Stored Procedures:
-use stored procedures to encapsulate sequences of SQL statements, enabling reusability and modularity in data transformation.

## External Functions & UDFs:
i) JavaScript UDFs(User-Defined Functions):
-allows the creation of UDFs using JavaScript, enabling custom logic for data transformation.
-functions can be used within SQL statements to perform more complex transformations not achievable by built-in.

## Snowflake's Partner ETL/ELT
i) Intergrations with ETL/ELT Tools:
-snowflakes intergrates with various 3rd party ETL/ELT tools like Matillion, Informatica, Talend, etc.
-tools offer drag & drop interfaces and workflows for designing data transformations. executed within SQL.

## Data Pipelines & Snowpipe
i) Data Pipelines:
-implement data pipelines using Snowpipe or others
-design workflows that include transformation steps along data ingestion or before loading data.

ii) External Data Transformation
-for more intricate transformations or special processing, data can be extracted from Snowflake using tools like Python, Spark etc. then loaded back to Snowflake.

# Basics of Data Modeling in Snowflake
-data modeling is the process of organizing and mapping data using simplified diagrams, symbols and text to represent data associations and flow.
-ensures the consistency and quality of data.
-differes from database schemas, data model is an overarching design determining what can exist in a schema.
-data modeler maps complex software system esigns into easy to understand diagrams.




