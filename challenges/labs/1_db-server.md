```
[root@ip-172-31-31-49 ec2-user]# hostname -f
ip-172-31-31-49.us-west-2.compute.internal
```

```
[root@ip-172-31-31-49 ec2-user]# mysql -u root -pcloudera -e "status;"
--------------
mysql  Ver 14.14 Distrib 5.5.59, for Linux (x86_64) using readline 5.1

Connection id:          12
Current database:
Current user:           root@localhost
SSL:                    Not in use
Current pager:          stdout
Using outfile:          ''
Using delimiter:        ;
Server version:         5.5.59 MySQL Community Server (GPL)
Protocol version:       10
Connection:             Localhost via UNIX socket
Server characterset:    latin1
Db     characterset:    latin1
Client characterset:    utf8
Conn.  characterset:    utf8
UNIX socket:            /var/lib/mysql/mysql.sock
Uptime:                 6 min 24 sec

Threads: 1  Questions: 48  Slow queries: 0  Opens: 34  Flush tables: 1  Open tables: 27  Queries per second avg: 0.125
```
```
[root@ip-172-31-31-49 ec2-user]# mysql -u root -pcloudera -e "show databases;"
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
+--------------------+
```
