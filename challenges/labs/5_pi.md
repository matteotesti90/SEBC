[bartfeld@ip-172-31-31-233 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 50 100
Number of Maps  = 50
Samples per Map = 100
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Wrote input for Map #16
Wrote input for Map #17
Wrote input for Map #18
Wrote input for Map #19
Wrote input for Map #20
Wrote input for Map #21
Wrote input for Map #22
Wrote input for Map #23
Wrote input for Map #24
Wrote input for Map #25
Wrote input for Map #26
Wrote input for Map #27
Wrote input for Map #28
Wrote input for Map #29
Wrote input for Map #30
Wrote input for Map #31
Wrote input for Map #32
Wrote input for Map #33
Wrote input for Map #34
Wrote input for Map #35
Wrote input for Map #36
Wrote input for Map #37
Wrote input for Map #38
Wrote input for Map #39
Wrote input for Map #40
Wrote input for Map #41
Wrote input for Map #42
Wrote input for Map #43
Wrote input for Map #44
Wrote input for Map #45
Wrote input for Map #46
Wrote input for Map #47
Wrote input for Map #48
Wrote input for Map #49
Starting Job
18/01/26 06:38:04 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-10.us-west-2.compute.internal/172.31.17.10:8032
18/01/26 06:38:04 INFO hdfs.DFSClient: Created token for bartfeld: HDFS_DELEGATION_TOKEN owner=bartfeld@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966684285, maxDate=1517571484285, sequenceNumber=3, masterKeyId=2 on 172.31.17.10:8020
18/01/26 06:38:04 INFO security.TokenCache: Got dt for hdfs://ip-172-31-17-10.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.10:8020, Ident: (token for bartfeld: HDFS_DELEGATION_TOKEN owner=bartfeld@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966684285, maxDate=1517571484285, sequenceNumber=3, masterKeyId=2)
18/01/26 06:38:04 INFO input.FileInputFormat: Total input paths to process : 50
18/01/26 06:38:04 INFO mapreduce.JobSubmitter: number of splits:50
18/01/26 06:38:04 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1516965730787_0003
18/01/26 06:38:04 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.10:8020, Ident: (token for bartfeld: HDFS_DELEGATION_TOKEN owner=bartfeld@MATTEOTESTI90.NEW, renewer=yarn, realUser=, issueDate=1516966684285, maxDate=1517571484285, sequenceNumber=3, masterKeyId=2)
18/01/26 06:38:05 INFO impl.YarnClientImpl: Submitted application application_1516965730787_0003
18/01/26 06:38:05 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-10.us-west-2.compute.internal:8088/proxy/application_1516965730787_0003/
18/01/26 06:38:05 INFO mapreduce.Job: Running job: job_1516965730787_0003
18/01/26 06:38:13 INFO mapreduce.Job: Job job_1516965730787_0003 running in uber mode : false
18/01/26 06:38:13 INFO mapreduce.Job:  map 0% reduce 0%
18/01/26 06:38:22 INFO mapreduce.Job:  map 2% reduce 0%
18/01/26 06:38:25 INFO mapreduce.Job:  map 4% reduce 0%
18/01/26 06:38:28 INFO mapreduce.Job:  map 8% reduce 0%
18/01/26 06:38:29 INFO mapreduce.Job:  map 10% reduce 0%
18/01/26 06:38:32 INFO mapreduce.Job:  map 12% reduce 0%
18/01/26 06:38:34 INFO mapreduce.Job:  map 14% reduce 0%
18/01/26 06:38:35 INFO mapreduce.Job:  map 16% reduce 0%
18/01/26 06:38:37 INFO mapreduce.Job:  map 18% reduce 0%
18/01/26 06:38:39 INFO mapreduce.Job:  map 20% reduce 0%
18/01/26 06:38:41 INFO mapreduce.Job:  map 22% reduce 0%
18/01/26 06:38:43 INFO mapreduce.Job:  map 24% reduce 0%
18/01/26 06:38:47 INFO mapreduce.Job:  map 26% reduce 0%
18/01/26 06:38:50 INFO mapreduce.Job:  map 28% reduce 0%
18/01/26 06:38:51 INFO mapreduce.Job:  map 32% reduce 0%
18/01/26 06:38:53 INFO mapreduce.Job:  map 34% reduce 0%
18/01/26 06:38:54 INFO mapreduce.Job:  map 36% reduce 0%
18/01/26 06:38:56 INFO mapreduce.Job:  map 38% reduce 0%
18/01/26 06:38:57 INFO mapreduce.Job:  map 42% reduce 0%
18/01/26 06:38:58 INFO mapreduce.Job:  map 44% reduce 0%
18/01/26 06:39:00 INFO mapreduce.Job:  map 46% reduce 0%
18/01/26 06:39:01 INFO mapreduce.Job:  map 48% reduce 0%
18/01/26 06:39:02 INFO mapreduce.Job:  map 52% reduce 0%
18/01/26 06:39:04 INFO mapreduce.Job:  map 54% reduce 0%
18/01/26 06:39:05 INFO mapreduce.Job:  map 56% reduce 0%
18/01/26 06:39:06 INFO mapreduce.Job:  map 60% reduce 0%
18/01/26 06:39:08 INFO mapreduce.Job:  map 62% reduce 0%
18/01/26 06:39:09 INFO mapreduce.Job:  map 64% reduce 0%
18/01/26 06:39:10 INFO mapreduce.Job:  map 68% reduce 0%
18/01/26 06:39:12 INFO mapreduce.Job:  map 70% reduce 0%
18/01/26 06:39:13 INFO mapreduce.Job:  map 72% reduce 0%
18/01/26 06:39:14 INFO mapreduce.Job:  map 78% reduce 0%
18/01/26 06:39:17 INFO mapreduce.Job:  map 80% reduce 0%
18/01/26 06:39:18 INFO mapreduce.Job:  map 82% reduce 0%
18/01/26 06:39:19 INFO mapreduce.Job:  map 84% reduce 0%
18/01/26 06:39:20 INFO mapreduce.Job:  map 88% reduce 0%
18/01/26 06:39:21 INFO mapreduce.Job:  map 90% reduce 0%
18/01/26 06:39:22 INFO mapreduce.Job:  map 92% reduce 0%
18/01/26 06:39:23 INFO mapreduce.Job:  map 96% reduce 0%
18/01/26 06:39:24 INFO mapreduce.Job:  map 98% reduce 0%
18/01/26 06:39:26 INFO mapreduce.Job:  map 100% reduce 100%
18/01/26 06:39:26 INFO mapreduce.Job: Job job_1516965730787_0003 completed successfully
18/01/26 06:39:26 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=261
                FILE: Number of bytes written=7676783
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=15040
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=203
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=50
                Launched reduce tasks=1
                Data-local map tasks=50
                Total time spent by all maps in occupied slots (ms)=157829
                Total time spent by all reduces in occupied slots (ms)=6852
                Total time spent by all map tasks (ms)=157829
                Total time spent by all reduce tasks (ms)=6852
                Total vcore-milliseconds taken by all map tasks=157829
                Total vcore-milliseconds taken by all reduce tasks=6852
                Total megabyte-milliseconds taken by all map tasks=161616896
                Total megabyte-milliseconds taken by all reduce tasks=7016448
        Map-Reduce Framework
                Map input records=50
                Map output records=100
                Map output bytes=900
                Map output materialized bytes=1700
                Input split bytes=9140
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=1700
                Reduce input records=100
                Reduce output records=0
                Spilled Records=200
                Shuffled Maps =50
                Failed Shuffles=0
                Merged Map outputs=50
                GC time elapsed (ms)=1164
                CPU time spent (ms)=24700
                Physical memory (bytes) snapshot=22935744512
                Virtual memory (bytes) snapshot=80891805696
                Total committed heap usage (bytes)=26347569152
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5900
        File Output Format Counters
                Bytes Written=97
Job Finished in 82.652 seconds
Estimated value of Pi is 3.14160000000000000000



