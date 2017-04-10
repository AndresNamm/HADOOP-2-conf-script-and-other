# List Of useful Commands
This tutorial is based on [MarkDown][md]



# TeraSort commands


yarn jar /opt/hadoop-2.6.0/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.6.0.jar teragen 10000000 /terainput1
yarn jar /opt/hadoop-2.6.0/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.6.0.jar teravalidate /terainput /teraoutputAndres
yarn jar /opt/hadoop-2.6.0/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.6.0.jar terasort /teraoutput /terasortAndres
yarn jar /opt/hadoop-2.6.0/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.6.0.jar terasort /terainput /teraoutputAndres -D mapreduce.job.reduces=3 -D mapreduce.reduce.memory.mb=250 -D mapreduce.task.io.sort.mb=150 -D mapreduce.reduce.shuffle.parallelcopies=8 -D mapreduce.job.reduce.slowstart.completemaps=0.33



# Ganglia Commands

ssh student13-x1 “sudo –S su - -c ‘service ganglia-monitor restart’”



[md]: http://www.markdowntutorial.com/conclusion/