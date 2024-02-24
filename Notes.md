
## Project Steps:

Establish an Amazon MWAA environment to securely orchestrate workflows with Apache Airflow, integrating it with Snowflake for data processing tasks.

Configure AWS Secrets Manager to securely store Snowflake credentials, ensuring safe authentication for workflow operations.

Implement three distinct Airflow DAGs to manage the data pipeline:

DAG1: Set up the MWAA connection to Snowflake, using the connection string stored in AWS Secrets Manager.
DAG2: Create necessary Snowflake objects, including databases, tables, storage integrations, and stages, to prepare for data handling.
DAG3: Execute the data pipeline, handling data from ingestion to transformation and analysis.
Utilize AWS S3 for storing and managing data, employing two separate buckets for raw and transformed data to streamline the data flow and simplify access for analysis.

Perform data transformation and analysis in Snowflake, leveraging its powerful cloud data platform capabilities to extract insights from the data.

Publish the results of the data analysis to Amazon Simple Notification Service (Amazon SNS) to enable consumption and action on the insights generated.

## Workflow

![Overview](/overview_solution.png)

## Project Files:

- ```Dags```: Contains the AirFlow Dag.
- ```Snowflake_queries```: Contains the SQL scripts that is used in the  AirFlow Dag.
- ```Output```: Contains screenshots of the final output. 
- ```Config```: Contains requirements.txt and snowflake config