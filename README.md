# Airflow Compose

This repo contains Docker Compose snippets for using Airflow with external Databases and with different brokers.

Setup Database Documentation - https://airflow.apache.org/docs/apache-airflow/stable/howto/set-up-database.html <br/>
Configuration Reference - https://airflow.apache.org/docs/apache-airflow/stable/configurations-ref.html

### How to use ?
Airflow needs to run initial migrations in order to setup Database for operations.

### Testing: <br/>
1) git clone https://github.com/OpsComb/Airflow-Compose.git
2) Run ```docker-compose up```
3) Open this url on your browser -> 127.0.0.1:8080
4) Login using -> username - airflow-user , password - airflow-user
> Note: docker-compose file at root is not recommended for production use cases

### Production: <br />
1) Head over to mysql(or postgres) depending upon the database service used.
2) Replace the placeholders (database host, user, password) with relevant values.
3) Run ```docker-compose up```
