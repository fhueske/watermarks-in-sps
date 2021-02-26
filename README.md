# Watermarks in Stream Processing Systems

This repository contains the [Apache Beam](https://beam.apache.org) pipeline that was used to benchmark the watermark 
subsystems of Google Cloud Dataflow and Apache Flink for the paper 

*"Watermarks in Stream Processing Systems: Semantics and Comparative Analysis of Apache Flink and Google Cloud 
Dataflow"* 

submitted for the Industrial Track of VLDB 2021 by Tyler Akidau, Edmon Begoli, Slava Chernyak, Fabian Hueske, 
Kathryn Knight, Kenneth Knowles, Daniel Mills, and Dan Sotolongo.

We plan to contribute this pipeline to the Apache Beam project.

## Requirements

* Java JDK >= 1.8 
* Apache Maven

## Build Instructions

* Apache Flink

```
mvn clean package -Pflink-runner
```

* Google Cloud Dataflow

```
mvn clean package -Pdataflow-runner
```

The executable JAR file is located at

```
./target/watermarks-in-sps-bundled-1.0.jar
```

Please see the Apache Beam documentation for instructions to submit the pipeline for execution to Apache Flink or 
Google Cloud Dataflow.