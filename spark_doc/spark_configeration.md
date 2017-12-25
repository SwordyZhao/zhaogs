# Spark 安裝配置
 
## 1.安裝Scalaj
 
 解壓安裝包；
 
在環境變量中添加如下：

'''
  export SCALA_HOME=/opt/scala
  export PATH=$SCALA_HOME/bin:$PATH
''' 
 
 測試是否安裝成功：
 
 scala -version
 
## 2.安裝spark：
 
解壓安裝包；
 
在 環境變量中田間如下：

'''
  export SCALA_HOME=/opt/spark
  export PATH=$SPARK_HOME/bin:$PATH
''' 
 
修改spark-env.sh文件：
```
export JAVA_HOME=/opt/java
export SCALA_HOME=/opt/scala
export HADOOP_HOME=/opt/hadoop
export HADOOP_CONF_DIR=/opt/hadoop/etc/hadoop     _hadoop的配置文件路徑_
export SPARK_MASTER_IP=192.168.1.1      *Master節點的ip地址*
export SPARK_WORKER_MEMORY=2g       *worker節點可以分配的最大的內存*
export SPARK_WORKER_CORES=2       *worker節點可以分配的最大核心數*
export SPARK_WORKER_INSTANCES=1   *每臺機器上開啟的Worker節點的數目*
```
啟動集群：
  
  spark/sbin下面的start-all.sh
  
兩個接口：

  8080：Spark的WebUI監聽接口
  
  7077：spark集群master的內部監聽接口
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
