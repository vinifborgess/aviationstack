# Aviation Data Engineering Project | Modern Data Engineering E2E Project
Using AviationStack API to obtain historical flight data and perform basic flight data processing and analysis.

# Problem Statement:
Obtain historical flight data and perform basic flight data processing and analysis.

# Architecture:
This architecture is designed/developed to be a robust and detailed product, standardized, and able to re-usability.



Step by Step Process Flow:
1)- API- lambda runs for real time flight, cities, airplanes and aircraft types and get data from Aviation stack.

2)- data get pushed to respective api stream and each stream has only 1 shard.

3)- once data pushed to stream then it gets consumed by kinesis firehose as per stream.

4)-kinesis has 300 seconds buffer time and data gets stored in S3.

5)-once data loaded in s3 then we run glue spark every hour for flight data and once in day for Citi, aircraft and airplane data.

6)- lambda and glue runs through cloud watch rules.

7)- table produced by glue job can be used in Athena and quickshight for analytics.

Architecture Diagram:
AWS Cloud Data Strivers Architecture

List of AWS services used:
Glue
Athena
Kinesis Firehose
Kinesis Data Streams
Lambda
Cloud Watch
S3
Quick Sight


