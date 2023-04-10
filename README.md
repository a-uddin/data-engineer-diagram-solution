# Data enginner system diagram

Solution Approach: <br/>
For this challenge, I propose an architecture that utilizes AWS services to create an efficient, reliable, and scalable pipeline to ingest data from trackman-backend to S3 data lake and dataengineering-db, while ensuring data is delivered within the specified time limits. I recommend using AWS Glue, Amazon CloudWatch, Amazon RDS, and Amazon S3.

Solution diagram is below: <br/>

<img src="https://github.com/a-uddin/data-engineer-diagram-solution/blob/main/TrackMan.png" width="724" height="520">

Components:


- AWS Glue Crawler: 
To ensure that data arrives in trackman-lake no later than 1 hour after it is first inserted into trackman-backend, AWS Glue can be set up to run on a schedule (schedule crawler), such as every 30 minutes, to extract and transform new data. AWS Glue can also be set up to monitor changes in the source database using change data capture (CDC) mechanisms. A Crawler can crawl multiple data stores in a single run.


- Glue Data Catalog: 
The crawler writes metadata to the Data Catalog. A table definition contains metadata about the data of trackman-backend. The table is written to a database, which is a container of tables in the Data Catalog. Attributes of a table include classification, which is a label created by the classifier that inferred the table schema.

- Glue Job: 
Glue job encapsulates a script that connects source data, processes it, and then writes it out to target data store. Typically, a job runs extract, transform, and load (ETL) scripts. Jobs can also run general-purpose Python scripts (Python shell jobs.) Glue triggers can start jobs based on a schedule or event, or on demand. Glue job run can be monitored to understand runtime metrics such as completion status, duration, and start time.
Glue jobs get data from Data catalog and targeted to S3 (trackman-lake) and RDS (dataengineering-db) 

- CloudWatch: CloudWatch will monitor the Glue job to ensure that the data arrives in trackman-lake within the specified time limits. CloudWatch will be used to trigger an alert if the Glue job fails to deliver data to trackman-lake.


- RDS: 
Dataengineering-db is a relational database that will be used as the backend for an internal application. AWS Glue will ingest data from trackman-backend and store it in dataengineering-db.


- S3: 
S3 data lake (trackman-lake) is used to store the ingested data in a suitable format for future use. This data can be used to create a data warehouse and make it available to analysts for reporting and analysis.

Notes:
- In the future, if we want to ingest data from some other data sources, we can use AWS Glue to extract and transform data from those sources and load it into this data lake.
- The data in the data lake will be stored in a suitable format for future use, which will enable efficient querying and analysis of data in the data warehouse.
- Amazon Redshift can be used as a data warehouse to make the data available to analysts for reporting and analysis. 
- For the query we can use Athena.
- We can use AWS CloudFormation to deploy this architecture, which will automate the provisioning and deployment of resources.
- This solution is scalable, maintainable, reliable, and cost-effective. It can handle data from multiple sources and can be easily extended in the future to include additional data sources and services as needed.
- With this architecture, data is ingested from trackman-backend, transformed and loaded into dataengineering-db and trackman-lake in a timely manner, and future data sources can be easily integrated into the pipeline.


