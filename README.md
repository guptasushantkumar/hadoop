HDFS federation
Block report vs edit log
use of different hdfs file systems
proxies for webhdfs
nfs & fuse



hadoop jar hadoopSamples/MaxTemparature.jar /user/sushant/1901 /user/sushant/output

start-dfs.sh
start-yarn.sh
mr-jobhistory-daemon.sh start historyserver
hadoop fs -rmr /user/sushant/seq1
hadoop jar $HADOOP_HOME/share/hadoop/mapreduce/hadoop-mapreduce-examples-*.jar sort -r 1 -inFormat org.apache.hadoop.mapreduce.lib.input.SequenceFileInputFormat -outFormat org.apache.hadoop.mapreduce.lib.output.SequenceFileOutputFormat -outKey org.apache.hadoop.io.IntWritable -outValue org.apache.hadoop.io.Text seq1 sorted
