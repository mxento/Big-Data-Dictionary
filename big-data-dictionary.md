# MX's Big Data Dictionary

A-Z Terms online: Peter James' Data Dictionary 
<https://peterjamesthomas.com/data-and-analytics-dictionary/>


The big data software list as how I currently understand it.

## The Hadoops
**Apache Hadoop (Vanilla)** : with hdfs storage. haddop is the distributed file store and data processing. It's like a regular database but spread about lots of linux boxes. There’s variants of hadoop similar to different linux os distros: Apache Hadoop (vanilla), MapR, Hbase, Cloudera, MongoDB.  
<https://en.wikipedia.org/wiki/Apache_Hadoop>

**Amazon EMR** : Amazon's cloud based implementation of various brands of hadoop (vanilla, MapR). Really fast to setup. One or 3 clicks to spin up a cluster and add spark or other apps. 
<https://aws.amazon.com/emr/>

**HortonWorks** : One of the most popular commercial company supported variety of hadoop. It's got tech support that large enterprises needs. <https://hortonworks.com/> 

**Cloudera** : The second most popular commercial company version of hadoop. This company is public and has a ticker.  <http://www.cloudera.com/> 

**MapR** : Also commercial; MapR claims to have full data protection, no single points of failure, improved performance, and dramatic ease of use. True replication.  
<https://en.wikipedia.org/wiki/MapR>

**HBase**
That is, it provides a fault-tolerant way of storing large quantities of sparse data. It's a NoSQL store.
<https://en.wikipedia.org/wiki/Apache_HBase>

**BigTable** : Compresses google's own big data filestore. powering Google cloud platform. So google's hadoop.
<https://en.wikipedia.org/wiki/Bigtable>

## Apps
**Apache Spark**: is an memory Haddoop App that does apparently everything. Spark which is gaining popularity. Spark is fast, probably why people like it. Spark Sql Spark Stream, everything’s growing.
It also has spark ML (machine learning) library.  
<http://spark.apache.org/>

**HCatalog**/**Hive** :
Similar to tables in RDS systems. Makes hadoop into a table like structure. Hive jobs supposedly isn't that fast.  
<https://cwiki.apache.org/confluence/display/Hive/HCatalog>

**Apache Kafka**: a popular open source pub/sub data brokering service also used for streaming. It does real-time processing and log aggregation and monitoring.  
<http://kafka.apache.org/> 

**Apache Storm**: Big time streaming processing of incoming big data. Or micro-batching. It does lambda function or what used to be transforms on datasets fast. 
<http://storm.apache.org/> 

**Flink** : Streaming data application that is faster than storm.  
<https://flink.apache.org/>


## Data Query
**Apache Hue**: web app gui for interfacing with Hadoop data stores. Like mysql workbench or sql server management studio.  
<https://en.wikipedia.org/wiki/Hue_(Hadoop)>

**Apache Presto** : Query data where it lives, including Hive, Cassandra, relational databases or even proprietary data stores. Facebook made it.  
<https://prestodb.io/>

**Drill** : SQL Query Engine for Hadoop, NoSQL and Cloud Storage. So it takes sql and create queries against hdfs stores. Fancy optimizer.
<https://en.wikipedia.org/wiki/Apache_Drill>

**Impala** : native (MPP) SQL query engine for Apache Hadoop.  
<http://impala.apache.org/>  
<https://en.wikipedia.org/wiki/Cloudera_Impala>

## Data Injestion 

**Apache Nifi**: Log collection service, used to collect IOT or similar volumes of data. Been around longer and has more enterprise users and support.
<https://nifi.apache.org/>



**StreamSets Dataflow **: Data injestion service, used to collect streams of data. Simple and lightweight. Vendor agnostic.
<https://streamsets.com/>

## Misc 

**Avro** : Data serializaion framework. Uses JSON. 
<https://en.wikipedia.org/wiki/Apache_Avro>


**Parquet** : Columar data store. encodes data to be smaller. 
<https://parquet.apache.org/> 

## Management

**Apache Zookeeper**: a cluster management software, open sourced. To manage all the different nodes’s and linux servers.
<https://zookeeper.apache.org/>  
<https://en.wikipedia.org/wiki/Apache_ZooKeeper>

**Apache Mesos**: The Mesos kernel runs on every machine and provides applications (e.g., Hadoop, Spark, Kafka, Elasticsearch) with resource management and scheduling across entire datacenter and cloud environments. so basically == Yarn 2.0.
<http://mesos.apache.org/>  
<https://en.wikipedia.org/wiki/Apache_Mesos>

**Oozie** : Workflow scheduler for haddop batch jobs. 
<https://en.wikipedia.org/wiki/Apache_Oozie>

**Apache Yarn** : Resource management of hadoop clusters. for optimal cluster utilization. 
<https://hadoop.apache.org/docs/r2.7.1/hadoop-yarn/hadoop-yarn-site/YARN.html>


**Bigtop** : Packaging, deployment and integeration testing. So some sort of dev ops framework for big data.  
<http://bigtop.apache.org/>


## Languages 

**MapReduce**: language/job to take run queries against hadoop. It’s syntax is hard; basically script how to jump between boxes and split data set and reduce the problem from a DAG. Lot of people prefer abstraction layer to do it. Hive is Sql based , which translates to map-reduce jobs. MR jobs are generally slow and does in big batches.  
<https://en.wikipedia.org/wiki/MapReduce>

**Pig** : platform language used to execute hadoop map reduce jobs that run in batch.
<https://en.wikipedia.org/wiki/Pig_(programming_tool)>

**Tez** : Does data processing like mapRduce but much faster. Used by netflix and facebook.
<https://tez.apache.org/> 

## ETL / Pipelining

**Sqoop** : Tool used to transfer data between hadoop and regular relational data stores. 
<http://sqoop.apache.org/> 

**Airflow** : Open source data engineering pipeline tool. Used to parallel etl data from nodes to target stores. AirBnb made it.
<http://airflow.incubator.apache.org/>

**Luigi**
Data piplines and complex etl jobs. Spotify made and uses it.
<https://github.com/spotify/luigi>



## Data Science/Machine Learning
**Mahout** : Scalable machine learning algorithm libraries. 
<https://en.wikipedia.org/wiki/Apache_Mahout>


## Data Visualizations

**Apache Druid**: In memory slice and dice cube that sits on top big data stores.  
<http://druid.io/>

**Kibana** : To have data visualization and reporting from the distributed systems. Same company as elastic search.    
<https://www.elastic.co/products/kibana>

## Distributed Search
**Lucene Search**:
Open Source information retrival libary. Basis of Solr and Elastic
<https://en.wikipedia.org/wiki/Lucene>

**Apache Solr** : Enterprise open source search through all the stuff.
<https://en.wikipedia.org/wiki/Apache_Solr>

**Elastic** : distributed searching of as Solr mostly. 
<https://en.wikipedia.org/wiki/Elasticsearch>

Comparison of the two:
>ES does offer less friction from the get-go and you feel like you have something working much quicker  
<http://solr-vs-elasticsearch.com/>


## NoSql key-value stores:

**MongoDB** : One of the most popular commercial NoSql vendors. It's got tech support that large enterprises needs.  
<https://www.mongodb.com/> 

**Cassandra** : Most reliable and super scalable data store of key-values. Structured data across many commodity servers, and no single point of failure. Columar too. Supposed to be pain to change the stucture.     
<http://cassandra.apache.org/>


**Apache Accumulo** : A sorted, distributed key/value store based on the Google BigTable. Accumulo has cell-level access labels and server-side programming mechanisms. NSA uses this as a high security Hadoop implementation. 
<https://accumulo.apache.org//>

 
**Redis** : in memory data store , good for caching hot data like websites, not a long term persistant data store.  
<http://redis.io/> 
