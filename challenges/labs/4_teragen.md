
[driscoll@ip-172-31-30-151 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=134217728 -Dmapreduce.job.maps=8 -Dmapreduce.map.memory.mb=1024 65536000 /user/driscoll/tgen
18/01/26 04:16:56 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-23-7.us-west-2.compute.internal/172.31.23.7:8032
18/01/26 04:16:57 INFO terasort.TeraSort: Generating 65536000 using 8
18/01/26 04:16:57 INFO mapreduce.JobSubmitter: number of splits:8
18/01/26 04:16:57 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
18/01/26 04:16:57 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1516957502620_0001
18/01/26 04:16:57 INFO impl.YarnClientImpl: Submitted application application_1516957502620_0001
18/01/26 04:16:57 INFO mapreduce.Job: The url to track the job: http://ip-172-31-23-7.us-west-2.compute.internal:8088/proxy/application_1516957502620_0001/
18/01/26 04:16:57 INFO mapreduce.Job: Running job: job_1516957502620_0001
18/01/26 04:17:02 INFO mapreduce.Job: Job job_1516957502620_0001 running in uber mode : false
18/01/26 04:17:03 INFO mapreduce.Job:  map 0% reduce 0%
18/01/26 04:17:14 INFO mapreduce.Job:  map 5% reduce 0%
18/01/26 04:17:15 INFO mapreduce.Job:  map 15% reduce 0%
18/01/26 04:17:17 INFO mapreduce.Job:  map 17% reduce 0%
18/01/26 04:17:18 INFO mapreduce.Job:  map 22% reduce 0%
18/01/26 04:17:20 INFO mapreduce.Job:  map 24% reduce 0%
18/01/26 04:17:21 INFO mapreduce.Job:  map 29% reduce 0%
18/01/26 04:17:23 INFO mapreduce.Job:  map 31% reduce 0%
18/01/26 04:17:24 INFO mapreduce.Job:  map 37% reduce 0%
18/01/26 04:17:26 INFO mapreduce.Job:  map 40% reduce 0%
18/01/26 04:17:27 INFO mapreduce.Job:  map 44% reduce 0%
18/01/26 04:17:29 INFO mapreduce.Job:  map 48% reduce 0%
18/01/26 04:17:30 INFO mapreduce.Job:  map 51% reduce 0%
18/01/26 04:17:32 INFO mapreduce.Job:  map 54% reduce 0%
18/01/26 04:17:33 INFO mapreduce.Job:  map 60% reduce 0%
18/01/26 04:17:34 INFO mapreduce.Job:  map 61% reduce 0%
18/01/26 04:17:35 INFO mapreduce.Job:  map 62% reduce 0%
18/01/26 04:17:36 INFO mapreduce.Job:  map 69% reduce 0%
18/01/26 04:17:38 INFO mapreduce.Job:  map 72% reduce 0%
18/01/26 04:17:39 INFO mapreduce.Job:  map 74% reduce 0%
18/01/26 04:17:40 INFO mapreduce.Job:  map 75% reduce 0%
18/01/26 04:17:43 INFO mapreduce.Job:  map 79% reduce 0%
18/01/26 04:17:46 INFO mapreduce.Job:  map 82% reduce 0%
18/01/26 04:17:47 INFO mapreduce.Job:  map 87% reduce 0%
18/01/26 04:17:49 INFO mapreduce.Job:  map 90% reduce 0%
18/01/26 04:17:50 INFO mapreduce.Job:  map 93% reduce 0%
18/01/26 04:17:52 INFO mapreduce.Job:  map 96% reduce 0%
18/01/26 04:17:53 INFO mapreduce.Job:  map 99% reduce 0%
18/01/26 04:17:54 INFO mapreduce.Job:  map 100% reduce 0%
18/01/26 04:17:54 INFO mapreduce.Job: Job job_1516957502620_0001 completed successfully
18/01/26 04:17:54 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=979408
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=682
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=32
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=8
                Other local map tasks=8
                Total time spent by all maps in occupied slots (ms)=232116
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=232116
                Total vcore-seconds taken by all map tasks=232116
                Total megabyte-seconds taken by all map tasks=237686784
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=682
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=751
                CPU time spent (ms)=104460
                Physical memory (bytes) snapshot=2514644992
                Virtual memory (bytes) snapshot=12633518080
                Total committed heap usage (bytes)=2717908992
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m0.290s
user    0m4.412s
sys     0m0.247s



[driscoll@ip-172-31-30-151 ~]$ hdfs dfs -ls /user/driscoll/tgen
Found 9 items
-rw-r--r--   3 driscoll driscoll          0 2018-01-26 04:17 /user/driscoll/tgen/_SUCCESS
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00000
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00001
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00002
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00003
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00004
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00005
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00006
-rw-r--r--   3 driscoll driscoll  819200000 2018-01-26 04:17 /user/driscoll/tgen/part-m-00007


[driscoll@ip-172-31-30-151 ~]$ hdfs fsck -blocks /user/driscoll/tgen/
Connecting to namenode via http://ip-172-31-23-7.us-west-2.compute.internal:50070
FSCK started by driscoll (auth:SIMPLE) from /172.31.30.151 for path /user/driscoll/tgen/ at Fri Jan 26 04:22:22 EST 2018
.........Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   9
 Total symlinks:                0
 Total blocks (validated):      56 (avg. block size 117028571 B)
 Minimally replicated blocks:   56 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Fri Jan 26 04:22:22 EST 2018 in 3 milliseconds
