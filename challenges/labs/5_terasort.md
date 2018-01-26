[driscoll@ip-172-31-31-233 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/driscoll/tgen /user/driscoll/tsort
18/01/26 06:33:38 INFO terasort.TeraSort: starting
18/01/26 06:33:39 INFO hdfs.DFSClient: Created token for driscoll: HDFS_DELEGATION_TOKEN owner=driscoll@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966419667, maxDate=1517571219667, sequenceNumber=2, masterKeyId=2 on 172.31.17.10:8020
18/01/26 06:33:39 INFO security.TokenCache: Got dt for hdfs://ip-172-31-17-10.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.10:8020, Ident: (token for driscoll: HDFS_DELEGATION_TOKEN owner=driscoll@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966419667, maxDate=1517571219667, sequenceNumber=2, masterKeyId=2)
18/01/26 06:33:39 INFO input.FileInputFormat: Total input paths to process : 8
Spent 263ms computing base-splits.
Spent 3ms computing TeraScheduler splits.
Computing input splits took 267ms
Sampling 10 splits of 56
Making 8 from 100000 sampled records
Computing parititions took 477ms
Spent 745ms computing partitions.
18/01/26 06:33:40 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-10.us-west-2.compute.internal/172.31.17.10:8032
18/01/26 06:33:40 INFO mapreduce.JobSubmitter: number of splits:56
18/01/26 06:33:40 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1516965730787_0002
18/01/26 06:33:40 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.10:8020, Ident: (token for driscoll: HDFS_DELEGATION_TOKEN owner=driscoll@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966419667, maxDate=1517571219667, sequenceNumber=2, masterKeyId=2)
18/01/26 06:33:41 INFO impl.YarnClientImpl: Submitted application application_1516965730787_0002
18/01/26 06:33:41 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-10.us-west-2.compute.internal:8088/proxy/application_1516965730787_0002/
18/01/26 06:33:41 INFO mapreduce.Job: Running job: job_1516965730787_0002
18/01/26 06:33:48 INFO mapreduce.Job: Job job_1516965730787_0002 running in uber mode : false
18/01/26 06:33:48 INFO mapreduce.Job:  map 0% reduce 0%
18/01/26 06:34:00 INFO mapreduce.Job:  map 4% reduce 0%
18/01/26 06:34:01 INFO mapreduce.Job:  map 11% reduce 0%
18/01/26 06:34:08 INFO mapreduce.Job:  map 14% reduce 0%
18/01/26 06:34:09 INFO mapreduce.Job:  map 21% reduce 0%
18/01/26 06:34:17 INFO mapreduce.Job:  map 25% reduce 0%
18/01/26 06:34:18 INFO mapreduce.Job:  map 32% reduce 0%
18/01/26 06:34:26 INFO mapreduce.Job:  map 36% reduce 0%
18/01/26 06:34:27 INFO mapreduce.Job:  map 43% reduce 0%
18/01/26 06:34:34 INFO mapreduce.Job:  map 45% reduce 0%
18/01/26 06:34:35 INFO mapreduce.Job:  map 48% reduce 0%
18/01/26 06:34:36 INFO mapreduce.Job:  map 54% reduce 0%
18/01/26 06:34:43 INFO mapreduce.Job:  map 55% reduce 0%
18/01/26 06:34:44 INFO mapreduce.Job:  map 57% reduce 0%
18/01/26 06:34:45 INFO mapreduce.Job:  map 61% reduce 0%
18/01/26 06:34:46 INFO mapreduce.Job:  map 64% reduce 0%
18/01/26 06:34:51 INFO mapreduce.Job:  map 66% reduce 0%
18/01/26 06:34:52 INFO mapreduce.Job:  map 68% reduce 0%
18/01/26 06:34:54 INFO mapreduce.Job:  map 71% reduce 0%
18/01/26 06:34:55 INFO mapreduce.Job:  map 75% reduce 0%
18/01/26 06:34:59 INFO mapreduce.Job:  map 79% reduce 0%
18/01/26 06:35:00 INFO mapreduce.Job:  map 82% reduce 0%
18/01/26 06:35:02 INFO mapreduce.Job:  map 84% reduce 0%
18/01/26 06:35:03 INFO mapreduce.Job:  map 88% reduce 0%
18/01/26 06:35:04 INFO mapreduce.Job:  map 89% reduce 0%
18/01/26 06:35:05 INFO mapreduce.Job:  map 93% reduce 0%
18/01/26 06:35:06 INFO mapreduce.Job:  map 95% reduce 0%
18/01/26 06:35:08 INFO mapreduce.Job:  map 96% reduce 0%
18/01/26 06:35:16 INFO mapreduce.Job:  map 98% reduce 0%
18/01/26 06:35:18 INFO mapreduce.Job:  map 98% reduce 4%
18/01/26 06:35:20 INFO mapreduce.Job:  map 98% reduce 8%
18/01/26 06:35:21 INFO mapreduce.Job:  map 98% reduce 16%
18/01/26 06:35:25 INFO mapreduce.Job:  map 98% reduce 20%
18/01/26 06:35:31 INFO mapreduce.Job:  map 98% reduce 25%
18/01/26 06:38:07 INFO mapreduce.Job:  map 98% reduce 20%
18/01/26 06:38:08 INFO mapreduce.Job:  map 98% reduce 16%
18/01/26 06:38:16 INFO mapreduce.Job:  map 100% reduce 16%
18/01/26 06:38:19 INFO mapreduce.Job:  map 100% reduce 21%
18/01/26 06:38:20 INFO mapreduce.Job:  map 100% reduce 27%
18/01/26 06:38:21 INFO mapreduce.Job:  map 100% reduce 40%
18/01/26 06:38:24 INFO mapreduce.Job:  map 100% reduce 42%
18/01/26 06:38:25 INFO mapreduce.Job:  map 100% reduce 48%
18/01/26 06:38:26 INFO mapreduce.Job:  map 100% reduce 50%
18/01/26 06:38:42 INFO mapreduce.Job:  map 100% reduce 60%
18/01/26 06:38:43 INFO mapreduce.Job:  map 100% reduce 71%
18/01/26 06:38:44 INFO mapreduce.Job:  map 100% reduce 81%
18/01/26 06:38:46 INFO mapreduce.Job:  map 100% reduce 83%
18/01/26 06:38:49 INFO mapreduce.Job:  map 100% reduce 85%
18/01/26 06:38:50 INFO mapreduce.Job:  map 100% reduce 86%
18/01/26 06:38:53 INFO mapreduce.Job:  map 100% reduce 88%
18/01/26 06:39:06 INFO mapreduce.Job:  map 100% reduce 98%
18/01/26 06:39:10 INFO mapreduce.Job:  map 100% reduce 100%
18/01/26 06:39:10 INFO mapreduce.Job: Job job_1516965730787_0002 completed successfully
18/01/26 06:39:10 INFO mapreduce.Job: Counters: 51
        File System Counters
                FILE: Number of bytes read=2916421633
                FILE: Number of bytes written=5790373527
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553608456
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=192
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Killed reduce tasks=2
                Launched map tasks=56
                Launched reduce tasks=10
                Data-local map tasks=54
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=405801
                Total time spent by all reduces in occupied slots (ms)=1228235
                Total time spent by all map tasks (ms)=405801
                Total time spent by all reduce tasks (ms)=1228235
                Total vcore-milliseconds taken by all map tasks=405801
                Total vcore-milliseconds taken by all reduce tasks=1228235
                Total megabyte-milliseconds taken by all map tasks=415540224
                Total megabyte-milliseconds taken by all reduce tasks=1257712640
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2864263352
                Input split bytes=8456
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2864263352
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =448
                Failed Shuffles=0
                Merged Map outputs=448
                GC time elapsed (ms)=7678
                CPU time spent (ms)=457580
                Physical memory (bytes) snapshot=38002307072
                Virtual memory (bytes) snapshot=101591601152
                Total committed heap usage (bytes)=45133332480
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
18/01/26 06:39:10 INFO terasort.TeraSort: done

real    5m33.292s
user    0m6.597s
sys     0m0.321s


