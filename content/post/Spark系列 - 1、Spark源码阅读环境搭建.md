---
title: 1、Spark源码阅读环境搭建
lastmod: 2025-04-26T13:37:55+08:00
draft: false
---

博主最近将开发环境从Mac切换到了Arch Linux，Mac由于需要用于办公，用起来总感觉不自在，一些涉及到公司的数据和代码，也不想和生活做交叉，因此希望能够进行物理机器层面的隔离。

这里进行简单的记录，方便下一次环境迁移。

## 一、基础环境搭建

需要安装的软件如下：
+  Spark 3.2.0
  链接地址：https://archive.apache.org/dist/spark/
+  Scala 2.12.15
+  Hadoop 3.2

```bash
# 源码
wget https://archive.apache.org/dist/spark/spark-3.2.0/spark-3.2.0.tgz
# bin程序
wget https://archive.apache.org/dist/spark/spark-3.2.0/spark-3.2.0-bin-hadoop3.2.tgz
# 对应的scala版本，2.12.15
wget https://downloads.lightbend.com/scala/2.12.15/scala-2.12.15.tgz
# 下载Hadoop 3.2
wget https://archive.apache.org/dist/hadoop/common/hadoop-3.2.2/hadoop-3.2.2.tar.gz
# 下载最新版本的maven
wget https://dlcdn.apache.org/maven/maven-3/3.9.9/binaries/apache-maven-3.9.9-bin.tar.gz

<mirror>
  <id>aliyunmaven</id>
  <mirrorOf>*</mirrorOf>
  <name>阿里云公共仓库</name>
  <url>https://maven.aliyun.com/repository/public</url>
</mirror>
```

