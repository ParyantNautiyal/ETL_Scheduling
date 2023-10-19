# ETL_Scheduling
Scheduling ETL Jobs Using Airflow.

Tech Stack: 
1. Pyspark
   :- To Transform The data ( Use Databricks or for practice use google colab)
2. Airflow
   :- To schedule the ETL jobs created using pyspark
3. AWS S3
   :- Used As Destination/Loading ( As Data Lake ) # NOTE Can use Redshift as Destination ( Data Warehouse)
4. Docker
   :-To Create a container using Airflow image # Edit config file before starting ( like comment out redis and flower) to reduce CPU and memory usage 
5. Power BI
   :- For Visualization
   
-- Using boto3 client to connect to AWS S3 .


-- Dataset : Air Travel and flight , containing Name ,Id ,Date OF travel , Flight taken ,Origin, Destination , Sex , Nationality and more .

-- Transformation : Standarization , removal of nulls( Filling out Null values) , Removing Duplicates , Creating aggregated dataframes for visualization


-- I Have Added a AWS_connect file , make changes accordingly provide path to file( Transfomed ) and add file at end of your code(Optional , you can run the file separatley or Add it Dags folder and make changes in dag.py to add Aws_connect). Don't FOrget to Save File in your system after Transformation done using pyspark .

-- Add dag.py and main.py( In this case I have uploaded a notebook ,Just use the code and create a main.py with proper folder structure..) in your Dags folder created( you may
   have to create the folder by yourself) before firing up the Airflow..

--  I have Added practice code in Notebook for pyspark 

# Have FUN
