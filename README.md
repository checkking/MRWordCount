# wordcount

### compile and package
mvn compile
mvn package	

### 运行程序
hadoop jar ./target/wordcount-0.0.1-SNAPSHOT.jar  com.stdatalabs.mapreduce.wordcount.WordCountDriver /wordcount/input/articles1.txt /wordcount/output/count_output /wordcount/output/sorted_output

### 上传数据集
hdfs dfs -mkdir /wordcount/output/
hdfs dfs -put ./articles1.txt /wordcount/input/