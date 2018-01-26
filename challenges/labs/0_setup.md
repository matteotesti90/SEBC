
Cloud provider AWS 

private IP
 172.31.31.49   ip-172-31-31-49.us-west-2.compute.internal
 172.31.30.151  ip-172-31-30-151.us-west-2.compute.internal
 172.31.31.233  ip-172-31-31-233.us-west-2.compute.internal
 172.31.27.173  ip-172-31-27-173.us-west-2.compute.internal
 172.31.23.7    ip-172-31-23-7.us-west-2.compute.internal
 
Public IP
 54.191.43.46 ec2-54-191-43-46.us-west-2.compute.amazonaws.com
 52.36.243.234 ec2-52-36-243-234.us-west-2.compute.amazonaws.com
 54.213.238.92 ec2-54-213-238-92.us-west-2.compute.amazonaws.com
 54.201.167.46 ec2-54-201-167-46.us-west-2.compute.amazonaws.com
 34.212.30.139 ec2-34-212-30-139.us-west-2.compute.amazonaws.com
 
Linux versione
 [root@ip-172-31-31-49 ec2-user]# uname -a
 Linux ip-172-31-31-49.us-west-2.compute.internal 3.10.0-327.36.3.el7.x86_64 #1 SMP Thu Oct 20 04:56:07 EDT 2016 x86_64 x86_64 x86_64 GNU/Linux

system capacity
[root@ip-172-31-31-49 ec2-user]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       50G  927M   50G   2% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.7G     0  7.7G   0% /dev/shm
tmpfs           7.7G   17M  7.7G   1% /run
tmpfs           7.7G     0  7.7G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/0
tmpfs           1.6G     0  1.6G   0% /run/user/1000


[root@ip-172-31-31-49 ec2-user]# yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                                                                                      | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                                                        | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                                                       | 3.8 kB  00:00:00
(1/7): rhui-REGION-client-config-server-7/x86_64/primary_db                                                             | 2.5 kB  00:00:00
(2/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/group                                                           |  104 B  00:00:00
(3/7): rhui-REGION-rhel-server-releases/7Server/x86_64/group                                                            | 709 kB  00:00:00
(4/7): rhui-REGION-rhel-server-releases/7Server/x86_64/updateinfo                                                       | 2.5 MB  00:00:00
(5/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/primary_db                                                      | 120 kB  00:00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/updateinfo                                                      |  33 kB  00:00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/primary_db                                                       |  47 MB  00:00:00
repo id                                                      repo name                                                                   status
rhui-REGION-client-config-server-7/x86_64                    Red Hat Update Infrastructure 2.0 Client Configuration Server 7                  1
rhui-REGION-rhel-server-releases/7Server/x86_64              Red Hat Enterprise Linux Server 7 (RPMs)                                    18,022
rhui-REGION-rhel-server-rh-common/7Server/x86_64             Red Hat Enterprise Linux Server 7 RH Common (RPMs)                             231
repolist: 18,254


[root@ip-172-31-31-49 ec2-user]# adduser -u 2650 driscoll
[root@ip-172-31-31-49 ec2-user]# adduser -u 3100 bartfeld
[root@ip-172-31-31-49 ec2-user]# groupadd intl
[root@ip-172-31-31-49 ec2-user]# groupadd americas
[root@ip-172-31-31-49 ec2-user]# usermod -a -G intl bartfeld
[root@ip-172-31-31-49 ec2-user]# usermod -a -G americas driscoll
[root@ip-172-31-31-49 ec2-user]# grep driscoll /etc/passwd
driscoll:x:2650:2650::/home/driscoll:/bin/bash
[root@ip-172-31-31-49 ec2-user]# grep bartfeld /etc/passwd
bartfeld:x:3100:3100::/home/bartfeld:/bin/bash
[root@ip-172-31-31-49 ec2-user]# grep intl /etc/group
intl:x:3101:bartfeld
[root@ip-172-31-31-49 ec2-user]# grep americas /etc/group
americas:x:3102:driscoll
