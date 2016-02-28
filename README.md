vagrant_hadoop
================================

# Introduction

Vagrant project to create a cluster of 4 virtual machines with Hadoop v2.4.1 and Spark v1.0.1. 

1. node1 : HDFS NameNode + Spark Master
2. node2 : YARN ResourceManager + JobHistoryServer + ProxyServer
3. node3 : HDFS DataNode + YARN NodeManager + Spark Slave
4. node4 : HDFS DataNode + YARN NodeManager + Spark Slave

# Requeriments

1. VirtualBox
2. Vagrant
3. Git clone this project,
4. Run ```vagrant up``` to create the VM.
5. Run ```vagrant ssh``` to get into your VM.
6. Run ```vagrant destroy``` when you want to destroy and get rid of the VM.

# Web Interface ( Monitoring )
You can check the following URLs to monitor the Hadoop daemons.

1. [NameNode] (http://10.211.55.101:50070/dfshealth.html)
2. [ResourceManager] (http://10.211.55.102:8088/cluster)
3. [JobHistory] (http://10.211.55.102:19888/jobhistory)
4. [Spark] (http://10.211.55.101:8080)