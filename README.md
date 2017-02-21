# Hadoop Benchmarks

A list of Hadoop Ecosystem Benchmark Links for reference 

HDFS

http://www.michael-noll.com/blog/2011/04/09/benchmarking-and-stress-testing-an-hadoop-cluster-with-terasort-testdfsio-nnbench-mrbench/ 

https://github.com/saurabhmishra/benchmarkhadoop 

TestDFSIO

Measure the I/O performance of HDFS in your cluster. Source code for the tool can be found here https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/fs/TestDFSIO.java 

HiBench 

https://github.com/intel-hadoop/HiBench 

NameNode Benchmark

Applies load on the namenode by performing continuous read, write, rename and delete operations on small files. Source code for this tool can be found here https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/hdfs/NNBench.java

Synthetic Load Generator

The synthetic load generator (SLG) is a tool for testing NameNode behavior under different client loads. The user can generate different mixes of read, write, and list requests by specifying the probabilities of read and write. The user controls the intensity of the load by adjusting parameters for the number of worker threads and the delay between operations. More information on the tool can be found here http://hadoop.apache.org/docs/r2.5.2/hadoop-project-dist/hadoop-hdfs/SLGUserGuide.html 

YARN/MR

TeraSort

Measure performance by measuring time to sort 1TB of data. The test runs in three steps. First one is TeraGen to generate the dataset, second one is the TeraSort to sort the generated data and third one is TeraValidate to verify the sort order is correct. You can change to use a different data size 

https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-examples/src/main/java/org/apache/hadoop/examples/terasort/TeraGen.java 

https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-examples/src/main/java/org/apache/hadoop/examples/terasort/TeraSort.java

https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-examples/src/main/java/org/apache/hadoop/examples/terasort/TeraValidate.java

https://community.hortonworks.com/content/kbentry/44315/teragen-terasort-and-teravalidate-performance-test.html 

MapReduce Benchmark

Runs a job multiple times and takes average of all runs. Source code for the tool can be found here 
https://github.com/apache/hadoop/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/mapred/MRBench.java 

https://github.com/sunileman/MapReduce-Performance_Testing 

GridMix

GridMix submits a mix of synthetic jobs, modeling a profile mined from production loads. More information on the tool can be found here 
https://hadoop.apache.org/docs/current/hadoop-gridmix/GridMix.html 

HBase

YCSB

Performance evaluation of HBase under pre-defined workloads. More information can be found here https://github.com/brianfrankcooper/YCSB/wiki 

HBase Performance Evaluation

Script used for evaluating HBase performance and scalability. Runs a HBase client that steps through one of a set of hardcoded tests or 'experiments' (e.g. a random reads test, a random writes test, etc.). More information can be found here 
https://wiki.apache.org/hadoop/Hbase/PerformanceEvaluation

LoadTest Tool

A command-line utility that reads, writes, and verifies data. Unlike PerformanceEvaluation, this tool validates the data written, and supports simultaneously writing and reading the same set of keys. Source for the tool can be found here 
https://github.com/apache/hbase/blob/master/hbase-server/src/test/java/org/apache/hadoop/hbase/util/LoadTestTool.java 

ChaosMonkey

A utility to injects faults in a running cluster. More information can be found here 
http://hbase.apache.org/0.94/book/hbase.tests.html 

Hive

TPC Benchmarks 

TPCDS and TPCH are analytic benchmarks that model generally applicable aspects of decision support system. Automated scripts to run TPC benchmarks at scale including the converted queries can be found here.
https://github.com/hortonworks/hive-testbench 

http://www.tpc.org/tpcx-hs/ 

Phoenix 

https://github.com/cartershanklin/phoenix-performance

Spark 

https://community.hortonworks.com/content/kbentry/56158/benchmark-your-hardware-for-hadoop-spark.html 

https://github.com/databricks/spark-sql-perf 

Kafka  

https://engineering.linkedin.com/kafka/benchmarking-apache-kafka-2-million-writes-second-three-cheap-machines
& 
https://gist.github.com/jkreps/c7ddb4041ef62a900e6c

