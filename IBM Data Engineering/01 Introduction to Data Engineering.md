# Introduction to Data Engineering  
## Data Engineering  
- Goal: Make quality data available for fact-finding and business decision-making.  
## Data Roles  
- Data  
    - DE  
    ![de](./static/de.png)  
    ![de_skills](./static/de_skills.png)  
    - DA  
    ![da](./static/da.png)  
    ![da_skills](./static/da_skills.png)  
    - DS  
    ![ds](./static/ds.png)  
    ![ds_skills](./static/ds_skills.png)  
    - BA/BI  
    ![ba](./static/ba.png)  
    ![bi](./static/bi.png)  
    - Roles  
    ![roles](./static/roles.png)  
- Data Engineering  
    - Data Warehouse Engineer  
    ![data_warehouse_engineer](./static/data_warehouse_engineer.png)  
    - Data Architect  
    ![data_architect](./static/data_architect.png)  
    - Data Manager  
    ![data_manager](./static/data_manager.png)  
    - Database Administrator  
    ![database_administrator](./static/database_administrator.png)  
    ![database_administrator1](./static/database_administrator1.png)  
    - Roles  
    ![de_roles](./static/de_roles.png)
- Data-related roles relationships
![roles_relationships](./static/roles_relationships.png)  
## DE Skills  
![functional_skills](./static/functional_skills.png)  
> - Data engineering requires a broad set of skillsets. 
> - **No one data engineer can possibly master each one of these skills**, which means you essentially need to **select one or more specialization areas**, but have a good understanding of all areas so that you can make more informed decisions. 
> - Your skills will grow over time with experience, the areas you choose to focus on, and the time you invest in upskilling yourself.  

1. OS  
![os_skills](./static/os_skills.png)  
2. Infrastructure Components  
![infrastructure_components_skills](./static/infrastructure_components_skills.png)  
3. Database  
![database_skills](./static/database_skills.png)  
4. Data Pipeline  
![data_pipeline_skills](./static/data_pipeline_skills.png)  
5. ETL Tools  
![etl_tools_skills](./static/etl_tools_skills.png)  
6. Language  
![language_skills](./static/language_skills.png)  
7. Big Data Process  
![big_data_process_tools](./static/big_data_process_tools.png)  
## Data Ecosystem  
- Data Repositories  
    > Data repositories help to isolate data and make reporting and analytics more efficient and credible while also serving as a data archive.  
    > - OLTP  
    > ![oltp](./static/oltp.png)  
    > - OLAP  
    > ![olap](./static/olap.png)  
    1. RDBMS
        > ACID: Atomicity, Consistensy, Isolation, Durability.  
    2. NoSQL  
        - Key-value store  
        - Document based  
        - Column based  
        - Graph based  
    3. Data Warehouses
        - A data warehouse is a central repository of data integrated from multiple sources.  
        - Data warehouses serve as the single source of truth, storing current and historical data that has been cleansed, conformed, and categorized.  
        - When data gets loaded into the data warehouse, it is already modeled and structured for a specific purpose, meaning it's analysis-ready.  
        - Architecture  
        ![data_warehouse_3tiers](./static/data_warehouse_3tiers.png)  
        - Vendors  
        ![data_warehouse_vendors](./static/data_warehouse_vendors.png)  
    4. Data Marts  
        ![data_marts](./static/data_marts.png)  
        - Dependent data marts are a sub-section of an enterprise data warehouse.  
        - Independent data marts are created from sources other than an enterprise data warehouse, such as internal operational systems or external data.  
        - Hybrid data marts combine inputs from data warehouses, operational systems, and external systems.  
        - Goals  
        ![data_mart_goals](./static/data_mart_goals.png)  
    5. Data Lakes  
        ![data_lake](./static/data_lake.png)  
        ![data_lake1](./static/data_lake1.png)  
## Big Data  
![big_data_the_vs](./static/big_data_the_vs.png)  
- Hadoop  
    - Hadoop is a collection of tools that provides distributed storage and processing of big data.  
    ![hadoop_hdfs](./static/hadoop_hdfs.png)  
- Hive  
    - Hive is a data warehouse for data query and analysis built on top of Hadoop.   
    ![hadoop_hive](./static/hadoop_hive.png)  
    ![hadoop_hive1](./static/hadoop_hive1.png)  
- Spark  
    - Spark is a distributed data analytics framework designed to perform complex data analytics in real-time.  
    ![hadoop_spark](./static/hadoop_spark.png)  
    ![hadoop_spark1](./static/hadoop_spark1.png)  
## Data Platform Architecture  
![data_platform_architecture](./static/data_platform_architecture.png)  
- Security  
    - The CIA Triad 
        ![the_cia_triad](./static/the_cia_triad.png)  
    - Physical Infrastructure Security  
    - Network Security  
    - Application Security  
    - Data Security  
## Data Engineering Lifecycle  
- Data wrangling
    - Data wrangling, also known as data munging, is an iterative process that involves data exploration, transformation, validation, and making data available for a credible and meaningful analysis.  
    - Data Wrangling involves a whole range of transformations and cleansing activities performed on the data. 
        - Transformation of raw data includes the tasks you undertake to:  
            - Structurally manipulate and combine data using Joins and Unions.  
            - Normalize data, that is, clean the database of unused and redundant data.  
            - Denormalize data, that is, combine data from multiple tables into a single table so that it can be queried faster.  
        - Cleansing activities include:  
            - Profiling data to uncover anomalies and quality issues.  
            - Visualizing data using statistical methods in order to spot outliers.  
            - Fixing issues such as missing values, duplicate data, irrelevant data, inconsistent formats, syntax errors, and outliers.  
> Imputation: calculates the missing value based on statistical values.  

- Performance tuning and troubleshooting  
    - Data Pipeline Performance Metrics  
    ![data_pipeline_performance_metrics](./static/data_pipeline_performance_metrics.png)  
    ![data_pipeline_performance_metrics1](./static/data_pipeline_performance_metrics1.png)  
    - Databases Performance Metrics  
    ![databases_performance_metrics](./static/databases_performance_metrics.png)  
    - Databases Optimization Practices  
    ![databases_performance_practices](./static/databases_performance_practices.png)  
    ![databases_performance_practices1](./static/databases_performance_practices1.png)  
- Governance and Compliance (治理 & 合规)  
    - Governance
        - Data Governance is a collection of principles, practices, and processes to maintain the security, privacy, and integrity of data through its lifecycle.  
        ![data_that_needs_governance](./static/data_that_needs_governance.png)  
        ![industry_specific_regulations](./static/industry_specific_regulations.png)  
    - Compliance
        ![compliance](./static/compliance.png)  
    - Governance and Compliance in Data Lifecycle
        - Compliance requires organizations to maintain an auditable trail of personal data through its lifecycle, which includes acquisition, processing, storage, sharing, retention, and disposal of data.  
        ![governance_&_compliance_in_data_lifecycle](./static/governance_&_compliance_in_data_lifecycle.png)  
        ![governance_&_compliance_in_data_lifecycle1](./static/governance_&_compliance_in_data_lifecycle1.png)  
        ![governance_&_compliance_in_data_lifecycle2](./static/governance_&_compliance_in_data_lifecycle2.png)  
        ![governance_&_compliance_in_data_lifecycle3](./static/governance_&_compliance_in_data_lifecycle3.png)  
        ![governance_&_compliance_in_data_lifecycle4](./static/governance_&_compliance_in_data_lifecycle4.png)  
    - Tools and technologies play a critical role in the implementation of a governance framework, offering features such as:  
        - Authentication and Access Control.  
        - Encryption and Data Masking.  
        - Hosting options that comply with requirements and restrictions for international data transfers.  
        - Monitoring and Alerting functionalities.  
        - Data erasure tools that ensure deleted data cannot be retrieved.  
- DataOps  
    - Gartner defines DataOps as a collaborative data management practice focused on improving the communication, integration, and automation of data flows between data managers and consumers across an organization.  
    - DataOps aims to create predictable delivery and change management of data, data models, and related artifacts.  
    - The purpose of the DataOps Methodology is to enable an organization to utilize a repeatable process to build and deploy analytics and data pipelines. 
    ![dataops](./static/dataops.png)  
    - The Establish DataOps Phase provides guidance on how to set up the organization for success in managing data.  
    - The Iterate DataOps Phase delivers the data for one defined sprint.  
    - The Improve DataOps Phase ensures learnings from each sprint is channeled back to continually improve the DataOps process.  
