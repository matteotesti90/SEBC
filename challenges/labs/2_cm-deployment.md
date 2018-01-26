the first line of CM server log

2018-01-26 03:44:53,692 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.11.2 (#6 built by jenkins on 20170811-0014 git: 3c3ea33a12076fb83a8f11c4452c52fac685d01b)

line in the log containing the string "Started Jetty server"

2018-01-26 03:45:54,983 INFO WebServerImpl:org.mortbay.log: jetty-6.1.26.cloudera.4
2018-01-26 03:45:54,984 INFO WebServerImpl:org.mortbay.log: Started SelectChannelConnector@0.0.0.0:7180
2018-01-26 03:45:54,984 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
2018-01-26 03:46:00,124 INFO ScmActive-0:com.cloudera.server.cmf.components.ScmActive: ScmActive completed successfully.
