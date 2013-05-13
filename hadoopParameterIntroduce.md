##Hadoop parameter intro
###Master and slave
* matser file: secondery namenode ip
* slave file: datenode and tasktracker ip  

###HDFS
* `fs.default.name` namenode's hostname and port,default is 8020
* `dfs.name.dir` directory of metadata (filesystem image)
   默认路径为：`${hadoop.tmp.dir}/dfs/name`
* `dfs.data.dir` directory for a datanode to store its blocks
   默认路径为：`${hadoop.tmp.dir}/dfs/data` 

###HDFS commond 
* hadoop fs -copyFromLocal 默认保存在 hdfs:// usr/lifeng/
