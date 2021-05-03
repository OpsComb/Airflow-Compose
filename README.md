# Airflow Compose

This repo contains Docker Compose snippets for using Airflow with external Databases and with different brokers.

Setup Database Documentation - https://airflow.apache.org/docs/apache-airflow/stable/howto/set-up-database.html <br/>
Configuration Reference - https://airflow.apache.org/docs/apache-airflow/stable/configurations-ref.html

### How to use ?
Airflow needs to run initial migrations in order to setup Database for operations.

For Testing: <br/>
Docker-compose at root path can be used for dev testing. It uses local database(postgres). 
** Note: docker-compose file at root is not recommended for production use cases

For Production:
1) Head over to mysql(or postgres) depending upon the database service used.
2) Replace the placeholders (database host, user, password) with relevant values.
3) Run ```docker-compose up```
