# Airflow_DAG_SeqExecutor

This repository focuses on the creation of a DAG (Directed Acyclic Graph) to schedule a Data Pipeline using Airflow. Docker is utilized to establish an environment with Airflow, wherein the Docker Compose file pulls the necessary Docker image and configures an Airflow Environment that facilitates DAG job scheduling.

To execute the code, docker-compose.yml file is to be run in the terminal. 
```
docker-compose up
```

## Project Architecture

![image](https://github.com/adithyang64/Airflow_DAG_SeqExecutor/assets/67658457/64845ef2-e277-4121-a12c-887c8421deb0)


## Description

This project uses raw data in the form of three CSV files containing information pertaining to hotels, clients, and bookings. The Python script is used for scheduling the DAG which can be found at /dags/data_ingestion_dag/main.py.

This specific script does the transformation of data from the raw CSV files and stores the processed data as CSV. Furthermore, it also loads the data into an SQLite database and stores in the filepath in .db format.
