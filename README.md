# ETL_Scheduling
Scheduling ETL Jobs Using Airflow.

Tech Stack: 
1. Pyspark
   :- To Transform The data
2. Airflow
   :- To schedule the ETL jobs created using pyspark
3. AWS S3
   :- Used As Destination/Loading ( As Data Lake ) # NOTE Can use Redshift as Destination ( Data Warehouse)
4. Docker
   :-To Create a container using Airflow image # Edit config file before starting ( like comment out redis and flower) to reduce CPU and memory usage 
5. Power BI
   :- For Visualization
-- Using boto3 client to connect to AWS S3 .


Dataset : Air Travel and flight , containing Name ,Id ,Date OF travel , Flight taken ,Origin, Destination , Sex , Nationality and more 
Transformation : Standarization , removal of nulls( Filling out Null values) , Removing Duplicates , Creating aggregated dataframes for visualization
