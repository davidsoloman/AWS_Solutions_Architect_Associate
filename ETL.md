1. extract data from data store  , transformed it to common format and load to central warehouse.
2. this led to new type of software called ETL => that integrate data between two systems
drawback - 
1. one global schema


Enterprise APplication Integration => thi was for strreaming
- used message buses
- did not scale u


both are dead

There is a new need due to scale for 
- high volume and divers
- event centric thinking needed
- ALlow forward compatible data architecture to scale for future need i.e to accomodate new data sources for data and new application to process
eg. moving from siggle DW to DW+CAssandra
but with stream only one cleaning


Requiremenr for modern data streaming


RAther than building platform on each tool
 
 
 Streaming p - serve as central nervous system
 
 ETL directly on Stream
 
 
 # Apache Kafka
 
 Role - 
 - storage choice for streaming
 - Append only log, reader use offset to read and scan ahead
 - huge read write
 
 
 Kafka stream API - transformation
 - offerer, filter ,joins maps
 
 - Fault tolerant local state
- Allow reprocessing -> eg. last 24 hour data-> data in kafka logs->
- Logs unify stream and batch as it combine stream over time batch = 1 day stream window

- Due to kafka log persistence and record offset, it is able to counter data backpressure in face of some breakdown
performance is stable as data can be made to persist


New release, June: Exactly one garuntee, this is good for Transactional data

security: SSL, ACL at topic level, client side security

types of data on Kafka:  Format and schema
- no strict schema : write in / write out,
- has now header support
- Have any schema if it can be put in message, Schema agnostic
-

Data redundancy and Failover - 
- Kafka is Replicated System , n time replication.
- support n-1 failure (master-slave architecture to pick after failure)

prev rec:
https://www.confluent.io/streaming-ingest-and-processing-with-kafka-webin/

have recording on->Confluent.io
    