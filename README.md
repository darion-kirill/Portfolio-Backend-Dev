# Java\Kotlin backend developer portfolio
___
## 1. Backend of a mobile application for servicing POS-terminals
While working at the Multikarta company, he was involved in support and development of the backend for a mobile application for engineers who service POS-terminals.

### Main functionality of the application:
- life cycle management of requests for configuration and repair of terminals
- building an optimal route (using GEO Api) to service points
- sending various types of notifications (SMS, push notifications, email notifications)
- building reports in various formats (PDF, Excel, XML, Word)

### What problems had to be solved:
- integration with GEO Api to build an optimal route on the map
- integration with the TranzWare Online banking transaction system
- setting up SSL and security on the server
- work with fiv and fiv to send push notifications to the mobile application
- generation of reports in the following formats: XLSX, DOCX, PDF (from HTML template)

Link to application: https://apps.rustore.ru/app/mk.mcc.android

___
## 2. Data quality system for working with client data (Customer Data Integration)
Work on a flagship enterprise high-load web application designed to standardize, process and store client data, as well as find duplicates in this data. The system is designed to work with client data of large businesses with tens of millions of clients in the banking and insurance sectors, retail and delivery services.

### Main functionality of the application:
- standardization of client data: addresses, phone numbers, client identification data (passport number), full name, email, etc.
- search for duplicates in source data using customizable rules
- checking clients using various stop lists
- calculation of client ratings, scoring
- notification of external consumers about changes in client data (RabbitMQ, Kafka)

### What problems had to be solved:
- implementation of various business logic: checking client data against the state tax register, depersonalization of outdated data using hashing, calculating the popularity of client data to further determine data quality, etc.
- implementation of a backend for an extensive administrative panel
- integration with various brokers: RabbitMQ, ActiveMQ, Apache Kafka
- security settings, role model
- optimization of work with Apache Lucene
- setting up pipelines

Link to product overview: https://hflabs.ru/uniform-client/

___
## 3. Client data masking system
Development of a new product for the HFLabs company - a system for masking client data while maintaining consistency and business sense. The system is subject to high requirements in terms of reliability, speed of operation and volume of processed simultaneous data.

### Main functionality of the application:
- provision of ETL processes with various types of connectors to SQL and NoSQL databases
- masking the main types of personal data using complex business logic, while maintaining the consistency and business meaning of the data
- caching masking results to maintain consistency
- finding sensitive information in source data based on business logic and NLP models

### What problems had to be solved:
- implementation of connectors with various types of databases: PostgreSQL, OracleDB, MySQL, MSSQL, Clickhouse, Greenplum, MongoDB, Elasticsearch
- implementation of a module that provides ETL-loaded processes
- integration with the NLP model to search for sensitive information in the source data
- building an architecture of microservices and their interaction with each other
- setting up continuous pipelines and deploying the application in Docker

Link to product overview: https://hflabs.ru/masking/