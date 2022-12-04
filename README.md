# bigdata-docker

# Docker Zeppelin

This repository contains [Apache Zeppelin 0.9.0](https://zeppelin.apache.org/) docker image, which is tuned to work with BDE clusters.

# Hadoop Docker


# Hive 
# Hive Docker
## Hive Interpreter for Apache Zeppelin
Hive Interpreter has been deprecated and merged into JDBC Interpreter. 
You can use Hive Interpreter by using JDBC Interpreter with same functionality. 
See the example below of settings and dependencies.

### Properties
<table class="table-configuration">
  <tr>
    <th>Property</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>default.driver</td>
    <td>org.apache.hive.jdbc.HiveDriver</td>
  </tr>
  <tr>
    <td>default.url</td>
    <td>jdbc:hive2://localhost:10000</td>
  </tr>
  <tr>
    <td>default.user</td>
    <td>hiveUser</td>
  </tr>
  <tr>
    <td>default.password</td>
    <td>hivePassword</td>
  </tr>
</table>

### Dependencies
<table class="table-configuration">
  <tr>
    <th>Artifact</th>
    <th>Exclude</th>
  </tr>
  <tr>
    <td>org.apache.hive:hive-jdbc:0.14.0</td>
    <td></td>
  </tr>
  <tr>
    <td>org.apache.hadoop:hadoop-common:2.6.0</td>
    <td></td>
  </tr>
</table>


### Configuration
<table class="table-configuration">
  <tr>
    <th>Property</th>
    <th>Default</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>default.driver</td>
    <td>org.apache.hive.jdbc.HiveDriver</td>
    <td>Class path of JDBC driver</td>
  </tr>
  <tr>
    <td>default.url</td>
    <td>jdbc:hive2://localhost:10000</td>
    <td>Url for connection</td>
  </tr>
  <tr>
    <td>default.user</td>
    <td></td>
    <td><b>( Optional ) </b>Username of the connection</td>
  </tr>
  <tr>
    <td>default.password</td>
    <td></td>
    <td><b>( Optional ) </b>Password of the connection</td>
  </tr>
  <tr>
    <td>default.xxx</td>
    <td></td>
    <td><b>( Optional ) </b>Other properties used by the driver</td>
  </tr>
  <tr>
    <td>zeppelin.jdbc.hive.timeout.threshold</td>
    <td>60000</td>
    <td>Timeout for hive job timeout</td>
  </tr>
  <tr>
    <td>zeppelin.jdbc.hive.monitor.query_interval</td>
    <td>1000</td>
    <td>Query interval for hive statement</td>
  </tr>
  <tr>
    <td>zeppelin.jdbc.hive.engines.tag.enable</td>
    <td>true</td>
    <td>Set application tag for applications started by hive engines</td>
  </tr>
</table>

# Spark 
# Spark Docker
## Connect Hive Interpreter With Spark in Apache Zeppelin
