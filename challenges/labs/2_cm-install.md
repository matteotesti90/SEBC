[root@ip-172-31-30-151 ec2-user]# yum -y install cloudera-manager-daemons cloudera-manager-server
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Resolving Dependencies
--> Running transaction check
---> Package cloudera-manager-daemons.x86_64 0:5.11.2-1.cm5112.p0.6.el7 will be installed
--> Processing Dependency: perl for package: cloudera-manager-daemons-5.11.2-1.cm5112.p0.6.el7.x86_64
---> Package cloudera-manager-server.x86_64 0:5.11.2-1.cm5112.p0.6.el7 will be installed
--> Running transaction check
---> Package perl.x86_64 4:5.16.3-292.el7 will be installed
--> Processing Dependency: perl-libs = 4:5.16.3-292.el7 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Scalar::Util) >= 1.10 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Socket) >= 1.3 for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Carp) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Cwd) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Exporter) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Path) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec::Functions) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Spec::Unix) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(File::Temp) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Filter::Util::Call) for package: 4:perl-5.16.3-292.el7.x86_64
--> Processing Dependency: perl(Getopt::Long) for package: 4:perl-5.16.3-292.el7.x86_64
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
--> Running transaction check
---> Package perl-Carp.noarch 0:1.26-244.el7 will be installed
---> Package perl-Exporter.noarch 0:5.68-3.el7 will be installed
---> Package perl-File-Path.noarch 0:2.09-2.el7 will be installed
---> Package perl-File-Temp.noarch 0:0.23.01-3.el7 will be installed
---> Package perl-Filter.x86_64 0:1.49-3.el7 will be installed
---> Package perl-Getopt-Long.noarch 0:2.40-2.el7 will be installed
--> Processing Dependency: perl(Pod::Usage) >= 1.14 for package: perl-Getopt-Long-2.40-2.el7.noarch
--> Processing Dependency: perl(Text::ParseWords) for package: perl-Getopt-Long-2.40-2.el7.noarch
---> Package perl-PathTools.x86_64 0:3.40-5.el7 will be installed
---> Package perl-Pod-Simple.noarch 1:3.28-4.el7 will be installed
--> Processing Dependency: perl(Pod::Escapes) >= 1.04 for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
--> Processing Dependency: perl(Encode) for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
---> Package perl-Scalar-List-Utils.x86_64 0:1.27-248.el7 will be installed
---> Package perl-Socket.x86_64 0:2.010-4.el7 will be installed
---> Package perl-Storable.x86_64 0:2.45-3.el7 will be installed
---> Package perl-Time-HiRes.x86_64 4:1.9725-3.el7 will be installed
---> Package perl-Time-Local.noarch 0:1.2300-2.el7 will be installed
---> Package perl-constant.noarch 0:1.27-2.el7 will be installed
---> Package perl-libs.x86_64 4:5.16.3-292.el7 will be installed
---> Package perl-macros.x86_64 4:5.16.3-292.el7 will be installed
---> Package perl-threads.x86_64 0:1.87-4.el7 will be installed
---> Package perl-threads-shared.x86_64 0:1.43-6.el7 will be installed
--> Running transaction check
---> Package perl-Encode.x86_64 0:2.51-7.el7 will be installed
---> Package perl-Pod-Escapes.noarch 1:1.04-292.el7 will be installed
---> Package perl-Pod-Usage.noarch 0:1.63-3.el7 will be installed
--> Processing Dependency: perl(Pod::Text) >= 3.15 for package: perl-Pod-Usage-1.63-3.el7.noarch
--> Processing Dependency: perl-Pod-Perldoc for package: perl-Pod-Usage-1.63-3.el7.noarch
---> Package perl-Text-ParseWords.noarch 0:3.29-4.el7 will be installed
--> Running transaction check
---> Package perl-Pod-Perldoc.noarch 0:3.20-4.el7 will be installed
--> Processing Dependency: perl(HTTP::Tiny) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
--> Processing Dependency: perl(parent) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
---> Package perl-podlators.noarch 0:2.5.1-3.el7 will be installed
--> Running transaction check
---> Package perl-HTTP-Tiny.noarch 0:0.033-3.el7 will be installed
---> Package perl-parent.noarch 1:0.225-244.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

===============================================================================================================================================
 Package                             Arch              Version                               Repository                                   Size
===============================================================================================================================================
Installing:
 cloudera-manager-daemons            x86_64            5.11.2-1.cm5112.p0.6.el7              cloudera-manager                            651 M
 cloudera-manager-server             x86_64            5.11.2-1.cm5112.p0.6.el7              cloudera-manager                            8.5 k
Installing for dependencies:
 perl                                x86_64            4:5.16.3-292.el7                      rhui-REGION-rhel-server-releases            8.0 M
 perl-Carp                           noarch            1.26-244.el7                          rhui-REGION-rhel-server-releases             19 k
 perl-Encode                         x86_64            2.51-7.el7                            rhui-REGION-rhel-server-releases            1.5 M
 perl-Exporter                       noarch            5.68-3.el7                            rhui-REGION-rhel-server-releases             28 k
 perl-File-Path                      noarch            2.09-2.el7                            rhui-REGION-rhel-server-releases             27 k
 perl-File-Temp                      noarch            0.23.01-3.el7                         rhui-REGION-rhel-server-releases             56 k
 perl-Filter                         x86_64            1.49-3.el7                            rhui-REGION-rhel-server-releases             76 k
 perl-Getopt-Long                    noarch            2.40-2.el7                            rhui-REGION-rhel-server-releases             56 k
 perl-HTTP-Tiny                      noarch            0.033-3.el7                           rhui-REGION-rhel-server-releases             38 k
 perl-PathTools                      x86_64            3.40-5.el7                            rhui-REGION-rhel-server-releases             83 k
 perl-Pod-Escapes                    noarch            1:1.04-292.el7                        rhui-REGION-rhel-server-releases             51 k
 perl-Pod-Perldoc                    noarch            3.20-4.el7                            rhui-REGION-rhel-server-releases             87 k
 perl-Pod-Simple                     noarch            1:3.28-4.el7                          rhui-REGION-rhel-server-releases            216 k
 perl-Pod-Usage                      noarch            1.63-3.el7                            rhui-REGION-rhel-server-releases             27 k
 perl-Scalar-List-Utils              x86_64            1.27-248.el7                          rhui-REGION-rhel-server-releases             36 k
 perl-Socket                         x86_64            2.010-4.el7                           rhui-REGION-rhel-server-releases             49 k
 perl-Storable                       x86_64            2.45-3.el7                            rhui-REGION-rhel-server-releases             77 k
 perl-Text-ParseWords                noarch            3.29-4.el7                            rhui-REGION-rhel-server-releases             14 k
 perl-Time-HiRes                     x86_64            4:1.9725-3.el7                        rhui-REGION-rhel-server-releases             45 k
 perl-Time-Local                     noarch            1.2300-2.el7                          rhui-REGION-rhel-server-releases             24 k
 perl-constant                       noarch            1.27-2.el7                            rhui-REGION-rhel-server-releases             19 k
 perl-libs                           x86_64            4:5.16.3-292.el7                      rhui-REGION-rhel-server-releases            688 k
 perl-macros                         x86_64            4:5.16.3-292.el7                      rhui-REGION-rhel-server-releases             43 k
 perl-parent                         noarch            1:0.225-244.el7                       rhui-REGION-rhel-server-releases             12 k
 perl-podlators                      noarch            2.5.1-3.el7                           rhui-REGION-rhel-server-releases            112 k
 perl-threads                        x86_64            1.87-4.el7                            rhui-REGION-rhel-server-releases             49 k
 perl-threads-shared                 x86_64            1.43-6.el7                            rhui-REGION-rhel-server-releases             39 k

Transaction Summary
===============================================================================================================================================
Install  2 Packages (+27 Dependent packages)

Total download size: 663 M
Installed size: 862 M
Downloading packages:
(1/29): perl-Encode-2.51-7.el7.x86_64.rpm                                                                               | 1.5 MB  00:00:00
(2/29): perl-5.16.3-292.el7.x86_64.rpm                                                                                  | 8.0 MB  00:00:00
(3/29): cloudera-manager-server-5.11.2-1.cm5112.p0.6.el7.x86_64.rpm                                                     | 8.5 kB  00:00:00
(4/29): perl-Exporter-5.68-3.el7.noarch.rpm                                                                             |  28 kB  00:00:00
(5/29): perl-File-Path-2.09-2.el7.noarch.rpm                                                                            |  27 kB  00:00:00
(6/29): perl-File-Temp-0.23.01-3.el7.noarch.rpm                                                                         |  56 kB  00:00:00
(7/29): perl-Filter-1.49-3.el7.x86_64.rpm                                                                               |  76 kB  00:00:00
(8/29): perl-Getopt-Long-2.40-2.el7.noarch.rpm                                                                          |  56 kB  00:00:00
(9/29): perl-Carp-1.26-244.el7.noarch.rpm                                                                               |  19 kB  00:00:00
(10/29): perl-HTTP-Tiny-0.033-3.el7.noarch.rpm                                                                          |  38 kB  00:00:00
(11/29): perl-PathTools-3.40-5.el7.x86_64.rpm                                                                           |  83 kB  00:00:00
(12/29): perl-Pod-Perldoc-3.20-4.el7.noarch.rpm                                                                         |  87 kB  00:00:00
(13/29): perl-Pod-Escapes-1.04-292.el7.noarch.rpm                                                                       |  51 kB  00:00:00
(14/29): perl-Pod-Simple-3.28-4.el7.noarch.rpm                                                                          | 216 kB  00:00:00
(15/29): perl-Scalar-List-Utils-1.27-248.el7.x86_64.rpm                                                                 |  36 kB  00:00:00
(16/29): perl-Pod-Usage-1.63-3.el7.noarch.rpm                                                                           |  27 kB  00:00:00
(17/29): perl-Socket-2.010-4.el7.x86_64.rpm                                                                             |  49 kB  00:00:00
(18/29): perl-Storable-2.45-3.el7.x86_64.rpm                                                                            |  77 kB  00:00:00
(19/29): perl-Text-ParseWords-3.29-4.el7.noarch.rpm                                                                     |  14 kB  00:00:00
(20/29): perl-Time-HiRes-1.9725-3.el7.x86_64.rpm                                                                        |  45 kB  00:00:00
(21/29): perl-Time-Local-1.2300-2.el7.noarch.rpm                                                                        |  24 kB  00:00:00
(22/29): perl-constant-1.27-2.el7.noarch.rpm                                                                            |  19 kB  00:00:00
(23/29): perl-libs-5.16.3-292.el7.x86_64.rpm                                                                            | 688 kB  00:00:00
(24/29): perl-macros-5.16.3-292.el7.x86_64.rpm                                                                          |  43 kB  00:00:00
(25/29): perl-parent-0.225-244.el7.noarch.rpm                                                                           |  12 kB  00:00:00
(26/29): perl-threads-1.87-4.el7.x86_64.rpm                                                                             |  49 kB  00:00:00
(27/29): perl-podlators-2.5.1-3.el7.noarch.rpm                                                                          | 112 kB  00:00:00
(28/29): perl-threads-shared-1.43-6.el7.x86_64.rpm                                                                      |  39 kB  00:00:00
(29/29): cloudera-manager-daemons-5.11.2-1.cm5112.p0.6.el7.x86_64.rpm                                                   | 651 MB  00:00:14
-----------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                           45 MB/s | 663 MB  00:00:14
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : 1:perl-parent-0.225-244.el7.noarch                                                                                         1/29
  Installing : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                          2/29
  Installing : perl-podlators-2.5.1-3.el7.noarch                                                                                          3/29
  Installing : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                         4/29
  Installing : 1:perl-Pod-Escapes-1.04-292.el7.noarch                                                                                     5/29
  Installing : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                     6/29
  Installing : perl-Encode-2.51-7.el7.x86_64                                                                                              7/29
  Installing : perl-Pod-Usage-1.63-3.el7.noarch                                                                                           8/29
  Installing : 4:perl-macros-5.16.3-292.el7.x86_64                                                                                        9/29
  Installing : 4:perl-libs-5.16.3-292.el7.x86_64                                                                                         10/29
  Installing : perl-Storable-2.45-3.el7.x86_64                                                                                           11/29
  Installing : perl-Exporter-5.68-3.el7.noarch                                                                                           12/29
  Installing : perl-constant-1.27-2.el7.noarch                                                                                           13/29
  Installing : perl-Time-Local-1.2300-2.el7.noarch                                                                                       14/29
  Installing : perl-Socket-2.010-4.el7.x86_64                                                                                            15/29
  Installing : perl-Carp-1.26-244.el7.noarch                                                                                             16/29
  Installing : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                     17/29
  Installing : perl-PathTools-3.40-5.el7.x86_64                                                                                          18/29
  Installing : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                19/29
  Installing : perl-File-Temp-0.23.01-3.el7.noarch                                                                                       20/29
  Installing : perl-File-Path-2.09-2.el7.noarch                                                                                          21/29
  Installing : perl-threads-shared-1.43-6.el7.x86_64                                                                                     22/29
  Installing : perl-threads-1.87-4.el7.x86_64                                                                                            23/29
  Installing : perl-Filter-1.49-3.el7.x86_64                                                                                             24/29
  Installing : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                       25/29
  Installing : perl-Getopt-Long-2.40-2.el7.noarch                                                                                        26/29
  Installing : 4:perl-5.16.3-292.el7.x86_64                                                                                              27/29
  Installing : cloudera-manager-daemons-5.11.2-1.cm5112.p0.6.el7.x86_64                                                                  28/29
  Installing : cloudera-manager-server-5.11.2-1.cm5112.p0.6.el7.x86_64                                                                   29/29
  Verifying  : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                                          1/29
  Verifying  : perl-threads-shared-1.43-6.el7.x86_64                                                                                      2/29
  Verifying  : perl-Storable-2.45-3.el7.x86_64                                                                                            3/29
  Verifying  : perl-Exporter-5.68-3.el7.noarch                                                                                            4/29
  Verifying  : perl-constant-1.27-2.el7.noarch                                                                                            5/29
  Verifying  : perl-PathTools-3.40-5.el7.x86_64                                                                                           6/29
  Verifying  : 4:perl-macros-5.16.3-292.el7.x86_64                                                                                        7/29
  Verifying  : cloudera-manager-daemons-5.11.2-1.cm5112.p0.6.el7.x86_64                                                                   8/29
  Verifying  : 1:perl-parent-0.225-244.el7.noarch                                                                                         9/29
  Verifying  : 4:perl-5.16.3-292.el7.x86_64                                                                                              10/29
  Verifying  : perl-File-Temp-0.23.01-3.el7.noarch                                                                                       11/29
  Verifying  : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                                                       12/29
  Verifying  : perl-Time-Local-1.2300-2.el7.noarch                                                                                       13/29
  Verifying  : 4:perl-libs-5.16.3-292.el7.x86_64                                                                                         14/29
  Verifying  : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                                        15/29
  Verifying  : perl-Socket-2.010-4.el7.x86_64                                                                                            16/29
  Verifying  : perl-Carp-1.26-244.el7.noarch                                                                                             17/29
  Verifying  : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                                                     18/29
  Verifying  : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                                                19/29
  Verifying  : 1:perl-Pod-Escapes-1.04-292.el7.noarch                                                                                    20/29
  Verifying  : perl-Pod-Usage-1.63-3.el7.noarch                                                                                          21/29
  Verifying  : perl-Encode-2.51-7.el7.x86_64                                                                                             22/29
  Verifying  : perl-podlators-2.5.1-3.el7.noarch                                                                                         23/29
  Verifying  : perl-Getopt-Long-2.40-2.el7.noarch                                                                                        24/29
  Verifying  : perl-File-Path-2.09-2.el7.noarch                                                                                          25/29
  Verifying  : perl-threads-1.87-4.el7.x86_64                                                                                            26/29
  Verifying  : perl-Filter-1.49-3.el7.x86_64                                                                                             27/29
  Verifying  : perl-Text-ParseWords-3.29-4.el7.noarch                                                                                    28/29
  Verifying  : cloudera-manager-server-5.11.2-1.cm5112.p0.6.el7.x86_64                                                                   29/29

Installed:
  cloudera-manager-daemons.x86_64 0:5.11.2-1.cm5112.p0.6.el7             cloudera-manager-server.x86_64 0:5.11.2-1.cm5112.p0.6.el7

Dependency Installed:
  perl.x86_64 4:5.16.3-292.el7                perl-Carp.noarch 0:1.26-244.el7              perl-Encode.x86_64 0:2.51-7.el7
  perl-Exporter.noarch 0:5.68-3.el7           perl-File-Path.noarch 0:2.09-2.el7           perl-File-Temp.noarch 0:0.23.01-3.el7
  perl-Filter.x86_64 0:1.49-3.el7             perl-Getopt-Long.noarch 0:2.40-2.el7         perl-HTTP-Tiny.noarch 0:0.033-3.el7
  perl-PathTools.x86_64 0:3.40-5.el7          perl-Pod-Escapes.noarch 1:1.04-292.el7       perl-Pod-Perldoc.noarch 0:3.20-4.el7
  perl-Pod-Simple.noarch 1:3.28-4.el7         perl-Pod-Usage.noarch 0:1.63-3.el7           perl-Scalar-List-Utils.x86_64 0:1.27-248.el7
  perl-Socket.x86_64 0:2.010-4.el7            perl-Storable.x86_64 0:2.45-3.el7            perl-Text-ParseWords.noarch 0:3.29-4.el7
  perl-Time-HiRes.x86_64 4:1.9725-3.el7       perl-Time-Local.noarch 0:1.2300-2.el7        perl-constant.noarch 0:1.27-2.el7
  perl-libs.x86_64 4:5.16.3-292.el7           perl-macros.x86_64 4:5.16.3-292.el7          perl-parent.noarch 1:0.225-244.el7
  perl-podlators.noarch 0:2.5.1-3.el7         perl-threads.x86_64 0:1.87-4.el7             perl-threads-shared.x86_64 0:1.43-6.el7

Complete!
