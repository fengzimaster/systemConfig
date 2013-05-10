##hadoop 伪分布式配置
### JAVA 环境配置
安装的是open-jdk，操作系统ubuntu12.04LTS，JAVA_HOME配置地址

* `JAVA_HOME=/usr/lib/jvm/java-6-openjdk-amd64`

### 安装SSH 
* `sudo apt-get install ssh`
* `ssh-keyagen -t rsa -P '' -f ~/.ssh/id_rsa`
* `cat ~/.ssh/id_rsa.pub >> ～/.ssh/authorized_keys`

### 下载并解压缩[hadoop](http://archive.apache.org/dist/hadoop/core/ "title")安装并配置
* core-site.xml
> ` <name>fs.default.name</name>
  <value>hdfs://localhost/</value>`
* hdfs-site.xml
>  ` <name>dfs.replication</name>
   <value>1</value>`
* mapred-site.xml
>  `<name>mapred.job.tracker</name>
   <value>localhost:8021</value>`

### 启动hadoop
* `start-all.sh`
* `stop-all.sh`
