[root@ip-172-31-31-49 ec2-user]# yum repolist enabled | grep mysql
mysql55-community/x86_64                         MySQL 5.5 Community Serv    376
[root@ip-172-31-31-49 ec2-user]# yum -y install mysql-community-server
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Resolving Dependencies
--> Running transaction check
---> Package mysql-community-server.x86_64 0:5.5.59-2.el7 will be installed
--> Processing Dependency: mysql-community-common(x86-64) = 5.5.59-2.el7 for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: mysql-community-client(x86-64) >= 5.5.8 for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(strict) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(Sys::Hostname) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(POSIX) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(Getopt::Long) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(File::Temp) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(File::Path) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(File::Copy) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(File::Basename) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(Data::Dumper) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(DBI) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.4)(64bit) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.1)(64bit) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: /usr/bin/perl for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Processing Dependency: libaio.so.1()(64bit) for package: mysql-community-server-5.5.59-2.el7.x86_64
--> Running transaction check
---> Package libaio.x86_64 0:0.3.109-13.el7 will be installed
---> Package mysql-community-client.x86_64 0:5.5.59-2.el7 will be installed
--> Processing Dependency: mysql-community-libs(x86-64) >= 5.5.8 for package: mysql-community-client-5.5.59-2.el7.x86_64
--> Processing Dependency: perl(Exporter) for package: mysql-community-client-5.5.59-2.el7.x86_64
---> Package mysql-community-common.x86_64 0:5.5.59-2.el7 will be installed
---> Package perl.x86_64 4:5.16.3-292.el7 will be installed
--> Processing Dependency: perl-libs = 4:5.16.3-292.el7 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Scalar::Util) >= 1.10 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Socket) >= 1.3 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Carp) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Cwd) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec::Functions) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec::Unix) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Filter::Util::Call) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Pod::Simple::Search) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Pod::Simple::XHTML) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Scalar::Util) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Socket) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Storable) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Time::HiRes) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Time::Local) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(constant) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(threads) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(threads::shared) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl-libs for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl-macros for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: libperl.so()(64bit) for package: 4:perl-5.16.3-292.el7.x86_64
---> Package perl-DBI.x86_64 0:1.627-4.el7 will be installed
--> Processing Dependency: perl(RPC::PlClient) >= 0.2000 for package: perl-DBI-1.627-4.el7.x86_64
--> Processing Dependency: perl(RPC::PlServer) >= 0.2001 for package: perl-DBI-1.627-4.el7.x86_64
---> Package perl-Data-Dumper.x86_64 0:2.145-3.el7 will be installed
---> Package perl-File-Path.noarch 0:2.09-2.el7 will be installed
---> Package perl-File-Temp.noarch 0:0.23.01-3.el7 will be installed
---> Package perl-Getopt-Long.noarch 0:2.40-2.el7 will be installed
--> Processing Dependency: perl(Pod::Usage) >= 1.14 for package: perl-Getopt-Long-2.40-2.el7.noarch
--> Processing Dependency: perl(Text::ParseWords) for package: perl-Getopt-Long-2.40-2.el7.noarch
--> Running transaction check
---> Package mariadb-libs.x86_64 1:5.5.50-1.el7_2 will be obsoleted
---> Package mysql-community-libs.x86_64 0:5.5.59-2.el7 will be obsoleting
---> Package perl-Carp.noarch 0:1.26-244.el7 will be installed
---> Package perl-Exporter.noarch 0:5.68-3.el7 will be installed
---> Package perl-Filter.x86_64 0:1.49-3.el7 will be installed
---> Package perl-PathTools.x86_64 0:3.40-5.el7 will be installed
---> Package perl-PlRPC.noarch 0:0.2020-14.el7 will be installed
--> Processing Dependency: perl(Net::Daemon) >= 0.13 for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Compress::Zlib) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Log) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Test) for package: perl-PlRPC-0.2020-14.el7.noarch
---> Package perl-Pod-Simple.noarch 1:3.28-4.el7 will be installed
--> Processing Dependency: perl(Pod::Escapes) >= 1.04 for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
--> Processing Dependency: perl(Encode) for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
---> Package perl-Pod-Usage.noarch 0:1.63-3.el7 will be installed
--> Processing Dependency: perl(Pod::Text) >= 3.15 for package: perl-Pod-Usage-1.63-3.el7.noarch
--> Processing Dependency: perl-Pod-Perldoc for package: perl-Pod-Usage-1.63-3.el7.noarch
---> Package perl-Scalar-List-Utils.x86_64 0:1.27-248.el7 will be installed
---> Package perl-Socket.x86_64 0:2.010-4.el7 will be installed
---> Package perl-Storable.x86_64 0:2.45-3.el7 will be installed
---> Package perl-Text-ParseWords.noarch 0:3.29-4.el7 will be installed
---> Package perl-Time-HiRes.x86_64 4:1.9725-3.el7 will be installed
---> Package perl-Time-Local.noarch 0:1.2300-2.el7 will be installed
---> Package perl-constant.noarch 0:1.27-2.el7 will be installed
---> Package perl-libs.x86_64 4:5.16.3-292.el7 will be installed
---> Package perl-macros.x86_64 4:5.16.3-292.el7 will be installed
---> Package perl-threads.x86_64 0:1.87-4.el7 will be installed
---> Package perl-threads-shared.x86_64 0:1.43-6.el7 will be installed
--> Running transaction check
---> Package perl-Encode.x86_64 0:2.51-7.el7 will be installed
---> Package perl-IO-Compress.noarch 0:2.061-2.el7 will be installed
--> Processing Dependency: perl(Compress::Raw::Bzip2) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
--> Processing Dependency: perl(Compress::Raw::Zlib) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
---> Package perl-Net-Daemon.noarch 0:0.48-5.el7 will be installed
---> Package perl-Pod-Escapes.noarch 1:1.04-292.el7 will be installed
---> Package perl-Pod-Perldoc.noarch 0:3.20-4.el7 will be installed
--> Processing Dependency: perl(HTTP::Tiny) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
--> Processing Dependency: perl(parent) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
---> Package perl-podlators.noarch 0:2.5.1-3.el7 will be installed
--> Running transaction check
---> Package perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7 will be installed
---> Package perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7 will be installed
---> Package perl-HTTP-Tiny.noarch 0:0.033-3.el7 will be installed
---> Package perl-parent.noarch 1:0.225-244.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

===============================================================================================================================================
 Package                              Arch                Version                          Repository                                     Size
===============================================================================================================================================
Installing:
 mysql-community-libs                 x86_64              5.5.59-2.el7                     mysql55-community                             1.8 M
     replacing  mariadb-libs.x86_64 1:5.5.50-1.el7_2
 mysql-community-server               x86_64              5.5.59-2.el7                     mysql55-community                              45 M
Installing for dependencies:
 libaio                               x86_64              0.3.109-13.el7                   rhui-REGION-rhel-server-releases               24 k
 mysql-community-client               x86_64              5.5.59-2.el7                     mysql55-community                              16 M
 mysql-community-common               x86_64              5.5.59-2.el7                     mysql55-community                             235 k
 perl                                 x86_64              4:5.16.3-292.el7                 rhui-REGION-rhel-server-releases              8.0 M
 perl-Carp                            noarch              1.26-244.el7                     rhui-REGION-rhel-server-releases               19 k
 perl-Compress-Raw-Bzip2              x86_64              2.061-3.el7                      rhui-REGION-rhel-server-releases               32 k
 perl-Compress-Raw-Zlib               x86_64              1:2.061-4.el7                    rhui-REGION-rhel-server-releases               57 k
 perl-DBI                             x86_64              1.627-4.el7                      rhui-REGION-rhel-server-releases              802 k
 perl-Data-Dumper                     x86_64              2.145-3.el7                      rhui-REGION-rhel-server-releases               47 k
 perl-Encode                          x86_64              2.51-7.el7                       rhui-REGION-rhel-server-releases              1.5 M
 perl-Exporter                        noarch              5.68-3.el7                       rhui-REGION-rhel-server-releases               28 k
 perl-File-Path                       noarch              2.09-2.el7                       rhui-REGION-rhel-server-releases               27 k
 perl-File-Temp                       noarch              0.23.01-3.el7                    rhui-REGION-rhel-server-releases               56 k
 perl-Filter                          x86_64              1.49-3.el7                       rhui-REGION-rhel-server-releases               76 k
 perl-Getopt-Long                     noarch              2.40-2.el7                       rhui-REGION-rhel-server-releases               56 k
 perl-HTTP-Tiny                       noarch              0.033-3.el7                      rhui-REGION-rhel-server-releases               38 k
 perl-IO-Compress                     noarch              2.061-2.el7                      rhui-REGION-rhel-server-releases              260 k
 perl-Net-Daemon                      noarch              0.48-5.el7                       rhui-REGION-rhel-server-releases               51 k
 perl-PathTools                       x86_64              3.40-5.el7                       rhui-REGION-rhel-server-releases               83 k
 perl-PlRPC                           noarch              0.2020-14.el7                    rhui-REGION-rhel-server-releases               36 k
 perl-Pod-Escapes                     noarch              1:1.04-292.el7                   rhui-REGION-rhel-server-releases               51 k
 perl-Pod-Perldoc                     noarch              3.20-4.el7                       rhui-REGION-rhel-server-releases               87 k
 perl-Pod-Simple                      noarch              1:3.28-4.el7                     rhui-REGION-rhel-server-releases              216 k
 perl-Pod-Usage                       noarch              1.63-3.el7                       rhui-REGION-rhel-server-releases               27 k
 perl-Scalar-List-Utils               x86_64              1.27-248.el7                     rhui-REGION-rhel-server-releases               36 k
 perl-Socket                          x86_64              2.010-4.el7                      rhui-REGION-rhel-server-releases               49 k
 perl-Storable                        x86_64              2.45-3.el7                       rhui-REGION-rhel-server-releases               77 k
 perl-Text-ParseWords                 noarch              3.29-4.el7                       rhui-REGION-rhel-server-releases               14 k
 perl-Time-HiRes                      x86_64              4:1.9725-3.el7                   rhui-REGION-rhel-server-releases               45 k
 perl-Time-Local                      noarch              1.2300-2.el7                     rhui-REGION-rhel-server-releases               24 k
 perl-constant                        noarch              1.27-2.el7                       rhui-REGION-rhel-server-releases               19 k
 perl-libs                            x86_64              4:5.16.3-292.el7                 rhui-REGION-rhel-server-releases              688 k
 perl-macros                          x86_64              4:5.16.3-292.el7                 rhui-REGION-rhel-server-releases               43 k
 perl-parent                          noarch              1:0.225-244.el7                  rhui-REGION-rhel-server-releases               12 k
 perl-podlators                       noarch              2.5.1-3.el7                      rhui-REGION-rhel-server-releases              112 k
 perl-threads                         x86_64              1.87-4.el7                       rhui-REGION-rhel-server-releases               49 k
 perl-threads-shared                  x86_64              1.43-6.el7                       rhui-REGION-rhel-server-releases               39 k

Transaction Summary
===============================================================================================================================================
Install  2 Packages (+37 Dependent packages)

Total download size: 76 M
Downloading packages:
(1/39): mysql-community-common-5.5.59-2.el7.x86_64.rpm                                                                  | 235 kB  00:00:00
(2/39): libaio-0.3.109-13.el7.x86_64.rpm                                                                                |  24 kB  00:00:00
(3/39): mysql-community-libs-5.5.59-2.el7.x86_64.rpm                                                                    | 1.8 MB  00:00:00
(4/39): perl-5.16.3-292.el7.x86_64.rpm                                                                                  | 8.0 MB  00:00:00
(5/39): perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64.rpm                                                                  |  32 kB  00:00:00
(6/39): perl-Carp-1.26-244.el7.noarch.rpm                                                                               |  19 kB  00:00:00
(7/39): perl-Compress-Raw-Zlib-2.061-4.el7.x86_64.rpm                                                                   |  57 kB  00:00:00
(8/39): perl-Data-Dumper-2.145-3.el7.x86_64.rpm                                                                         |  47 kB  00:00:00
(9/39): perl-DBI-1.627-4.el7.x86_64.rpm                                                                                 | 802 kB  00:00:00
(10/39): perl-Encode-2.51-7.el7.x86_64.rpm                                                                              | 1.5 MB  00:00:00
(11/39): perl-Exporter-5.68-3.el7.noarch.rpm                                                                            |  28 kB  00:00:00
(12/39): perl-File-Path-2.09-2.el7.noarch.rpm                                                                           |  27 kB  00:00:00
(13/39): perl-File-Temp-0.23.01-3.el7.noarch.rpm                                                                        |  56 kB  00:00:00
(14/39): perl-Filter-1.49-3.el7.x86_64.rpm                                                                              |  76 kB  00:00:00
(15/39): perl-Getopt-Long-2.40-2.el7.noarch.rpm                                                                         |  56 kB  00:00:00
(16/39): perl-HTTP-Tiny-0.033-3.el7.noarch.rpm                                                                          |  38 kB  00:00:00
(17/39): perl-IO-Compress-2.061-2.el7.noarch.rpm                                                                        | 260 kB  00:00:00
(18/39): perl-Net-Daemon-0.48-5.el7.noarch.rpm                                                                          |  51 kB  00:00:00
(19/39): perl-PathTools-3.40-5.el7.x86_64.rpm                                                                           |  83 kB  00:00:00
(20/39): perl-Pod-Escapes-1.04-292.el7.noarch.rpm                                                                       |  51 kB  00:00:00
(21/39): perl-Pod-Perldoc-3.20-4.el7.noarch.rpm                                                                         |  87 kB  00:00:00
(22/39): perl-PlRPC-0.2020-14.el7.noarch.rpm                                                                            |  36 kB  00:00:00
(23/39): perl-Pod-Simple-3.28-4.el7.noarch.rpm                                                                          | 216 kB  00:00:00
(24/39): perl-Pod-Usage-1.63-3.el7.noarch.rpm                                                                           |  27 kB  00:00:00
(25/39): perl-Scalar-List-Utils-1.27-248.el7.x86_64.rpm                                                                 |  36 kB  00:00:00
(26/39): perl-Socket-2.010-4.el7.x86_64.rpm                                                                             |  49 kB  00:00:00
(27/39): perl-Storable-2.45-3.el7.x86_64.rpm                                                                            |  77 kB  00:00:00
(28/39): perl-Text-ParseWords-3.29-4.el7.noarch.rpm                                                                     |  14 kB  00:00:00
(29/39): perl-Time-HiRes-1.9725-3.el7.x86_64.rpm                                                                        |  45 kB  00:00:00
(30/39): perl-Time-Local-1.2300-2.el7.noarch.rpm                                                                        |  24 kB  00:00:00
(31/39): perl-constant-1.27-2.el7.noarch.rpm                                                                            |  19 kB  00:00:00
(32/39): mysql-community-client-5.5.59-2.el7.x86_64.rpm                                                                 |  16 MB  00:00:01
(33/39): perl-libs-5.16.3-292.el7.x86_64.rpm                                                                            | 688 kB  00:00:00
(34/39): perl-macros-5.16.3-292.el7.x86_64.rpm                                                                          |  43 kB  00:00:00
(35/39): perl-parent-0.225-244.el7.noarch.rpm                                                                           |  12 kB  00:00:00
(36/39): perl-threads-1.87-4.el7.x86_64.rpm                                                                             |  49 kB  00:00:00
(37/39): perl-podlators-2.5.1-3.el7.noarch.rpm                                                                          | 112 kB  00:00:00
(38/39): perl-threads-shared-1.43-6.el7.x86_64.rpm                                                                      |  39 kB  00:00:00
(39/39): mysql-community-server-5.5.59-2.el7.x86_64.rpm                                                                 |  45 MB  00:00:02
-----------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                           22 MB/s |  76 MB  00:00:03
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : mysql-community-common-5.5.59-2.el7.x86_64                                                                                 1/40
  Installing : mysql-community-libs-5.5.59-2.el7.x86_64                                                                                   2/40
  Installing : 1:perl-parent-0.225-244.el7.noarch                                                                                         3/40
  Installing : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                          4/40
  Installing : perl-podlators-2.5.1-3.el7.noarch                                                                                          5/40
  Installing : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                         6/40
  Installing : 1:perl-Pod-Escapes-1.04-292.el7.noarch                                                                                     7/40
  Installing : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                     8/40
  Installing : perl-Encode-2.51-7.el7.x86_64                                                                                              9/40
  Installing : perl-Pod-Usage-1.63-3.el7.noarch                                                                                          10/40
  Installing : 4:perl-macros-5.16.3-292.el7.x86_64                                                                                       11/40
  Installing : 4:perl-libs-5.16.3-292.el7.x86_64                                                                                         12/40
  Installing : perl-Storable-2.45-3.el7.x86_64                                                                                           13/40
  Installing : perl-Exporter-5.68-3.el7.noarch                                                                                           14/40
  Installing : perl-Socket-2.010-4.el7.x86_64                                                                                            15/40
  Installing : perl-Carp-1.26-244.el7.noarch                                                                                             16/40
  Installing : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                     17/40
  Installing : perl-PathTools-3.40-5.el7.x86_64                                                                                          18/40
  Installing : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                19/40
  Installing : perl-Time-Local-1.2300-2.el7.noarch                                                                                       20/40
  Installing : perl-constant-1.27-2.el7.noarch                                                                                           21/40
  Installing : perl-File-Temp-0.23.01-3.el7.noarch                                                                                       22/40
  Installing : perl-File-Path-2.09-2.el7.noarch                                                                                          23/40
  Installing : perl-threads-shared-1.43-6.el7.x86_64                                                                                     24/40
  Installing : perl-threads-1.87-4.el7.x86_64                                                                                            25/40
  Installing : perl-Filter-1.49-3.el7.x86_64                                                                                             26/40
  Installing : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                       27/40
  Installing : perl-Getopt-Long-2.40-2.el7.noarch                                                                                        28/40
  Installing : 4:perl-5.16.3-292.el7.x86_64                                                                                              29/40
  Installing : perl-Data-Dumper-2.145-3.el7.x86_64                                                                                       30/40
  Installing : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                                                31/40
  Installing : perl-Net-Daemon-0.48-5.el7.noarch                                                                                         32/40
  Installing : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                                               33/40
  Installing : perl-IO-Compress-2.061-2.el7.noarch                                                                                       34/40
  Installing : perl-PlRPC-0.2020-14.el7.noarch                                                                                           35/40
  Installing : perl-DBI-1.627-4.el7.x86_64                                                                                               36/40
  Installing : mysql-community-client-5.5.59-2.el7.x86_64                                                                                37/40
  Installing : libaio-0.3.109-13.el7.x86_64                                                                                              38/40
  Installing : mysql-community-server-5.5.59-2.el7.x86_64                                                                                39/40
  Erasing    : 1:mariadb-libs-5.5.50-1.el7_2.x86_64                                                                                      40/40
  Verifying  : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                          1/40
  Verifying  : perl-threads-shared-1.43-6.el7.x86_64                                                                                      2/40
  Verifying  : perl-Storable-2.45-3.el7.x86_64                                                                                            3/40
  Verifying  : perl-IO-Compress-2.061-2.el7.noarch                                                                                        4/40
  Verifying  : perl-Exporter-5.68-3.el7.noarch                                                                                            5/40
  Verifying  : perl-PathTools-3.40-5.el7.x86_64                                                                                           6/40
  Verifying  : 4:perl-macros-5.16.3-292.el7.x86_64                                                                                        7/40
  Verifying  : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                                                 8/40
  Verifying  : 1:perl-parent-0.225-244.el7.noarch                                                                                         9/40
  Verifying  : perl-Net-Daemon-0.48-5.el7.noarch                                                                                         10/40
  Verifying  : 4:perl-5.16.3-292.el7.x86_64                                                                                              11/40
  Verifying  : perl-File-Temp-0.23.01-3.el7.noarch                                                                                       12/40
  Verifying  : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                       13/40
  Verifying  : perl-Time-Local-1.2300-2.el7.noarch                                                                                       14/40
  Verifying  : 4:perl-libs-5.16.3-292.el7.x86_64                                                                                         15/40
  Verifying  : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                        16/40
  Verifying  : perl-DBI-1.627-4.el7.x86_64                                                                                               17/40
  Verifying  : libaio-0.3.109-13.el7.x86_64                                                                                              18/40
  Verifying  : perl-Socket-2.010-4.el7.x86_64                                                                                            19/40
  Verifying  : perl-Carp-1.26-244.el7.noarch                                                                                             20/40
  Verifying  : perl-Data-Dumper-2.145-3.el7.x86_64                                                                                       21/40
  Verifying  : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                     22/40
  Verifying  : mysql-community-libs-5.5.59-2.el7.x86_64                                                                                  23/40
  Verifying  : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                24/40
  Verifying  : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                                               25/40
  Verifying  : 1:perl-Pod-Escapes-1.04-292.el7.noarch                                                                                    26/40
  Verifying  : mysql-community-client-5.5.59-2.el7.x86_64                                                                                27/40
  Verifying  : perl-Pod-Usage-1.63-3.el7.noarch                                                                                          28/40
  Verifying  : perl-PlRPC-0.2020-14.el7.noarch                                                                                           29/40
  Verifying  : perl-Encode-2.51-7.el7.x86_64                                                                                             30/40
  Verifying  : perl-podlators-2.5.1-3.el7.noarch                                                                                         31/40
  Verifying  : perl-Getopt-Long-2.40-2.el7.noarch                                                                                        32/40
  Verifying  : perl-constant-1.27-2.el7.noarch                                                                                           33/40
  Verifying  : perl-File-Path-2.09-2.el7.noarch                                                                                          34/40
  Verifying  : perl-threads-1.87-4.el7.x86_64                                                                                            35/40
  Verifying  : mysql-community-common-5.5.59-2.el7.x86_64                                                                                36/40
  Verifying  : perl-Filter-1.49-3.el7.x86_64                                                                                             37/40
  Verifying  : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                    38/40
  Verifying  : mysql-community-server-5.5.59-2.el7.x86_64                                                                                39/40
  Verifying  : 1:mariadb-libs-5.5.50-1.el7_2.x86_64                                                                                      40/40

Installed:
  mysql-community-libs.x86_64 0:5.5.59-2.el7                            mysql-community-server.x86_64 0:5.5.59-2.el7

Dependency Installed:
  libaio.x86_64 0:0.3.109-13.el7                 mysql-community-client.x86_64 0:5.5.59-2.el7   mysql-community-common.x86_64 0:5.5.59-2.el7
  perl.x86_64 4:5.16.3-292.el7                   perl-Carp.noarch 0:1.26-244.el7                perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7
  perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7    perl-DBI.x86_64 0:1.627-4.el7                  perl-Data-Dumper.x86_64 0:2.145-3.el7
  perl-Encode.x86_64 0:2.51-7.el7                perl-Exporter.noarch 0:5.68-3.el7              perl-File-Path.noarch 0:2.09-2.el7
  perl-File-Temp.noarch 0:0.23.01-3.el7          perl-Filter.x86_64 0:1.49-3.el7                perl-Getopt-Long.noarch 0:2.40-2.el7
  perl-HTTP-Tiny.noarch 0:0.033-3.el7            perl-IO-Compress.noarch 0:2.061-2.el7          perl-Net-Daemon.noarch 0:0.48-5.el7
  perl-PathTools.x86_64 0:3.40-5.el7             perl-PlRPC.noarch 0:0.2020-14.el7              perl-Pod-Escapes.noarch 1:1.04-292.el7
  perl-Pod-Perldoc.noarch 0:3.20-4.el7           perl-Pod-Simple.noarch 1:3.28-4.el7            perl-Pod-Usage.noarch 0:1.63-3.el7
  perl-Scalar-List-Utils.x86_64 0:1.27-248.el7   perl-Socket.x86_64 0:2.010-4.el7               perl-Storable.x86_64 0:2.45-3.el7
  perl-Text-ParseWords.noarch 0:3.29-4.el7       perl-Time-HiRes.x86_64 4:1.9725-3.el7          perl-Time-Local.noarch 0:1.2300-2.el7
  perl-constant.noarch 0:1.27-2.el7              perl-libs.x86_64 4:5.16.3-292.el7              perl-macros.x86_64 4:5.16.3-292.el7
  perl-parent.noarch 1:0.225-244.el7             perl-podlators.noarch 0:2.5.1-3.el7            perl-threads.x86_64 0:1.87-4.el7
  perl-threads-shared.x86_64 0:1.43-6.el7

Replaced:
  mariadb-libs.x86_64 1:5.5.50-1.el7_2

Complete!
