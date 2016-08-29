# MX's big data dictionary

This Open Source big data software list as how I currently understand it.

**Hadoop** : hdfs is the basic distributed file store; like a database but spread about lots of linux boxes. Many things run on top of it. Best of which is Spark which is gaining popularity.
There’s variants of hadoop similar to different linux os distros: Apache Hadoop (vanilla), MapR, Hbase, Cloudera, MongoDB. I don’t know the differences too well.

**MapReduce**: language/job to take run queries against hadoop. It’s syntax is hard; basically script how to jump between boxes and split data set and reduce the problem from a DAG. Lot of people prefer abstraction layer to do it. Hive is Sql based , which translates to map-reduce jobs. MR jobs are generally slow and does in big batches.

**Apache Spark**: is an memory Haddoop App that does apparently everything. Spark is fast, probably why people like it. Spark Sql Spark Stream, everything’s growing.
It also has spark ML (machine learning) library.

**Apache Kafka**: a popular open source pub/sub data brokering service also used for streaming. It does real-time processing and log aggregation and monitoring.

**Apache Zookeeper**: a cluster management software, open sourced. To manage all the different nodes’s and linux servers.

**Apache Mesos**: The Mesos kernel runs on every machine and provides applications (e.g., Hadoop, Spark, Kafka, Elasticsearch) with resource management and scheduling across entire datacenter and cloud environments. so basically == Yarn 2.0.

**Apache Storm**: Big time streaming processing of incoming big data. It does lambda function or what used to be transforms on datasets fast.

**Apache Druid **: In memory slice and dice cube that sits on top big data stores.

**Kibana** : to have data visualization and reporting from the distributed systems.

**Airflow** : Open source data engineering pipeline tool. Used to parallel etl data from nodes to target stores. AirBnb made it.

**Apache Nifi **: Log collection service, used to collect IOT or similar volumes of data.

**Apache Hue**: web app gui for interfacing with Hadoop data stores.

**Apache Lucene Search**:
**Apache Solr** : open source search through all the stuff.
**Elastic Search** : distributed searching of nosql json same as Solr mostly

NoSql key-value stores:

**Cassandra** : Most reliable and super scalable data store of key-values. Very hard to analytics on.
Redis : in memory data store , good for caching hot data like websites, not a long term data store.
 
**Drill** :

**Flink** :

**Yarn** :

**Pig** :

**Mahout** :

**Tez**,

**Parquet** :

**Impala** :

**Sqoop** :

**Avro** :

**Oozie** :

**Bigtop** :

**HCatalog** :

**Luigi**