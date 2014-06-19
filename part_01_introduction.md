# Dive into Solr

A tutorial is also available from the [Apache Solr website](http://lucene.apache.org/solr/tutorial.html). This tutorial is focused on a simple use case which will be more familiar to people working in libraries.

## Prerequisites

This tutorial doesn't assume any technological expertise, but familiarity with the follwing will be helpful:

* xml syntax
* your operating system command line intereface
* text file editing
* the characteristics of metadata

Java JDK, minimum 6 or 7, depending the version of Solr you're using. This tutorial was developed with Solr 4.8.1, which is compatible with Java 7. To download the Java JDK, please see instructions on [Oracle's site](http://www.oracle.com/technetwork/java/javase/downloads/index.html).

You should be able to run the command `java -version` from your command line and see output similar to this:

```
java version "1.7.0_60"
Java(TM) SE Runtime Environment (build 1.7.0_60-b19)
Java HotSpot(TM) 64-Bit Server VM (build 24.60-b09, mixed mode)
```

## Steps

* [Install Solr](part_02_setup.md)
* Start and stop Solr
* Load some sample data into Solr 
* Explore the admin and browse interfaces
* Get some Dublin Core sample data
* Edit schema.xml for indexing the sample data
* Define solrconfig.xml for quering the sample data
