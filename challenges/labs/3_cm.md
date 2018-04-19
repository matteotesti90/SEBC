```
[root@ip-172-31-30-151 ec2-user]# hdfs dfs -ls /user
Found 8 items
drwxr-xr-x   - admin    admin               0 2018-01-26 04:08 /user/admin
drwxr-xr-x   - bartfeld bartfeld            0 2018-01-26 04:09 /user/bartfeld
drwxr-xr-x   - driscoll driscoll            0 2018-01-26 04:09 /user/driscoll
drwxr-xr-x   - hdfs     supergroup          0 2018-01-26 04:08 /user/hdfs
drwxrwxrwx   - mapred   hadoop              0 2018-01-26 04:05 /user/history
drwxrwxr-t   - hive     hive                0 2018-01-26 04:05 /user/hive
drwxrwxr-x   - hue      hue                 0 2018-01-26 04:06 /user/hue
drwxrwxr-x   - oozie    oozie               0 2018-01-26 04:06 /user/oozie
```

```
[root@ip-172-31-30-151 ec2-user]# curl -u admin:admin 'http://52.36.243.234:7180/api/v8/hosts'
{
  "items" : [ {
    "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee",
    "ipAddress" : "172.31.23.7",
    "hostname" : "ip-172-31-23-7.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/hostRedirect/5571542f-92d1-42e8-99a0-0189f72e83ee",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 16388911104
  }, {
    "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853",
    "ipAddress" : "172.31.27.173",
    "hostname" : "ip-172-31-27-173.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/hostRedirect/888b01fb-fc59-4f20-b5fb-f4a7f1ee3853",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 16388911104
  }, {
    "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d",
    "ipAddress" : "172.31.30.151",
    "hostname" : "ip-172-31-30-151.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/hostRedirect/4eb63078-8e1d-4f18-9631-f0b07781229d",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 16388911104
  }, {
    "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620",
    "ipAddress" : "172.31.31.233",
    "hostname" : "ip-172-31-31-233.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/hostRedirect/f73e829a-ab67-4436-9c99-28484e3f9620",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 16388911104
  }, {
    "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302",
    "ipAddress" : "172.31.31.49",
    "hostname" : "ip-172-31-31-49.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/hostRedirect/169d76a2-39be-41a5-8ec3-89678a3f1302",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 16388911104
  } ]


[root@ip-172-31-30-151 ec2-user]# curl -u admin:admin 'http://52.36.243.234:7180/api/v11/clusters/matteotesti90/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hbase",
    "type" : "HBASE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hbase",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hbase/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HBASE_MASTER_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HBASE_REGION_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HBase",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "roleInstancesUrl" : "http://ip-172-31-30-151.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS",
    "entityStatus" : "GOOD_HEALTH"
  } ]



[root@ip-172-31-30-151 ec2-user]# curl -u admin:admin 'http://52.36.243.234:7180/api/v16/cm/deployment'
{
  "timestamp" : "2018-01-26T09:11:47.310Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "matteotesti90",
    "version" : "CDH5",
    "fullVersion" : "5.8.5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hbase_service",
          "value" : "hbase",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-31-49.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password",
          "sensitive" : true
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-140587b9a1450f38c280428ba06a0879",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-a8ec9af26780ed870f164d190f1ef501",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-be1897e8706888a00ac528e729a29663",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-d3ca5cb9676f8e6f5ba1083fb2cfae89",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-be1897e8706888a00ac528e729a29663",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "endefnb0gnjjxvb2d7difn3hc",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6z9ye7oidiijvyy5znnm9l48y",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
        }
      } ],
      "displayName" : "Hive",
      "roleConfigGroups" : [ {
        "name" : "hive-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-BASE",
        "displayName" : "Hive Metastore Server Default Group",
        "roleType" : "HIVEMETASTORE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1983905792",
            "sensitive" : false
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "198390579",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-BASE",
        "displayName" : "HiveServer2 Default Group",
        "roleType" : "HIVESERVER2",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1717567488",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "985766297",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "165",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-BASE",
        "displayName" : "WebHCat Server Default Group",
        "roleType" : "WEBHCAT",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "replicationSchedules" : [ ]
    }, {
      "name" : "hbase",
      "type" : "HBASE",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hbase-MASTER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "MASTER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ao5suut8s1y40yqaxkye9rjjx",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-MASTER-BASE"
        }
      }, {
        "name" : "hbase-REGIONSERVER-140587b9a1450f38c280428ba06a0879",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4o9ihvntip6eo6i7jw8b8mke7",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-1"
        }
      }, {
        "name" : "hbase-REGIONSERVER-a8ec9af26780ed870f164d190f1ef501",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "87x55wtketc0ls9ojtd5idy29",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-2"
        }
      }, {
        "name" : "hbase-REGIONSERVER-be1897e8706888a00ac528e729a29663",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "14cq954e9j8bvgzia7jvro32w",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-BASE"
        }
      }, {
        "name" : "hbase-REGIONSERVER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9r24qch3lhavo969yzy6m4ksy",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-3"
        }
      } ],
      "displayName" : "HBase",
      "roleConfigGroups" : [ {
        "name" : "hbase-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-HBASERESTSERVER-BASE",
        "displayName" : "HBase REST Server Default Group",
        "roleType" : "HBASERESTSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-HBASETHRIFTSERVER-BASE",
        "displayName" : "HBase Thrift Server Default Group",
        "roleType" : "HBASETHRIFTSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-MASTER-BASE",
        "displayName" : "Master Default Group",
        "roleType" : "MASTER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-1",
        "displayName" : "RegionServer Group 1",
        "roleType" : "REGIONSERVER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "2287992832",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-2",
        "displayName" : "RegionServer Group 2",
        "roleType" : "REGIONSERVER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "1715470336",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-3",
        "displayName" : "RegionServer Group 3",
        "roleType" : "REGIONSERVER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "892338176",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-BASE",
        "displayName" : "RegionServer Default Group",
        "roleType" : "REGIONSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "1983905792",
            "sensitive" : false
          } ]
        }
      } ],
      "snapshotPolicies" : [ ]
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-140587b9a1450f38c280428ba06a0879",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "eygyssgr14h2a5xcfvtyo7jkk",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "3",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7lyhd5l18nfmrrez05vc6orbm",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "2",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-a8ec9af26780ed870f164d190f1ef501",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "114ox2mwttnmi31movo8msti1",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "1",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      } ],
      "displayName" : "ZooKeeper",
      "roleConfigGroups" : [ {
        "name" : "zookeeper-SERVER-BASE",
        "displayName" : "Server Default Group",
        "roleType" : "SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "zookeeper"
        },
        "config" : {
          "items" : [ {
            "name" : "maxSessionTimeout",
            "value" : "60000",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-31-49.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "database_password",
          "value" : "hue_password",
          "sensitive" : true
        }, {
          "name" : "database_type",
          "value" : "mysql",
          "sensitive" : false
        }, {
          "name" : "hbase_service",
          "value" : "hbase",
          "sensitive" : false
        }, {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-625b156b33850a0b0c4170dcec6fd65e",
          "sensitive" : false
        }, {
          "name" : "oozie_service",
          "value" : "oozie",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5yu52jilr3qft4vuuxwxgi3rf",
            "sensitive" : true
          }, {
            "name" : "secret_key",
            "value" : "HxAMVTQtDnOQ1V3dj0EFaSMfCuxuQS",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_SERVER-BASE"
        }
      } ],
      "displayName" : "Hue",
      "roleConfigGroups" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-BASE",
        "displayName" : "Load Balancer Default Group",
        "roleType" : "HUE_LOAD_BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-HUE_SERVER-BASE",
        "displayName" : "Hue Server Default Group",
        "roleType" : "HUE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-KT_RENEWER-BASE",
        "displayName" : "Kerberos Ticket Renewer Default Group",
        "roleType" : "KT_RENEWER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aye5j7ud87d01cbcfziihspc7",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "oozie-OOZIE_SERVER-BASE"
        }
      } ],
      "displayName" : "Oozie",
      "roleConfigGroups" : [ {
        "name" : "oozie-OOZIE_SERVER-BASE",
        "displayName" : "Oozie Server Default Group",
        "roleType" : "OOZIE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "oozie"
        },
        "config" : {
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-31-49.us-west-2.compute.internal",
            "sensitive" : false
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password",
            "sensitive" : true
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql",
            "sensitive" : false
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "9hFryND6VJJTMuduYQbMlPW9xULzhG",
          "sensitive" : true
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7elxq7n1udtpe7hvuo09rpfkr",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-140587b9a1450f38c280428ba06a0879",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2yl7t3pk20mzrx620s8c8gcu6",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-a8ec9af26780ed870f164d190f1ef501",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4g6gqtrwaachnlyzbdzjkih1g",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-2"
        }
      }, {
        "name" : "yarn-NODEMANAGER-be1897e8706888a00ac528e729a29663",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aaihgwemndkitu2zv28ptqsvw",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2q9tdh4hl38h8e7v7k49su38l",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-3"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "63",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "3yrdddkshveej3zeohwzkpdnv",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-RESOURCEMANAGER-BASE"
        }
      } ],
      "displayName" : "YARN (MR2 Included)",
      "roleConfigGroups" : [ {
        "name" : "yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8",
            "sensitive" : false
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-JOBHISTORY-BASE",
        "displayName" : "JobHistory Server Default Group",
        "roleType" : "JOBHISTORY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1",
        "displayName" : "NodeManager Group 1",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "2836",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2",
        "displayName" : "NodeManager Group 2",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "2127",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-3",
        "displayName" : "NodeManager Group 3",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "node_manager_java_heapsize",
            "value" : "892338176",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1106",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-BASE",
        "displayName" : "NodeManager Default Group",
        "roleType" : "NODEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "2460",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-BASE",
        "displayName" : "ResourceManager Default Group",
        "roleType" : "RESOURCEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "2836",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "Sr1ATpUCtUnSAWioCxR0xjky1rbZrr",
          "sensitive" : true
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "aZ7ZA6V47O5DTIgNTQX9JDVgZnZ1gT",
          "sensitive" : true
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "C5axq4tPchdkHihK2ct7rx8388sSW6",
          "sensitive" : true
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-140587b9a1450f38c280428ba06a0879",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3cibkzxt6aaade8rdthr6i4fe",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-a8ec9af26780ed870f164d190f1ef501",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6v28um16nog6axngugj1ctg45",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-2"
        }
      }, {
        "name" : "hdfs-DATANODE-be1897e8706888a00ac528e729a29663",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "an1xna2dda1hu29jh2v1fdls4",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-d3ca5cb9676f8e6f5ba1083fb2cfae89",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "702tt6lnwkupcq702ve8ucu25",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-3"
        }
      }, {
        "name" : "hdfs-NAMENODE-625b156b33850a0b0c4170dcec6fd65e",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "65",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "f2necir3kj7yab84ftlzlyjqz",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-a8ec9af26780ed870f164d190f1ef501",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f1dqs5t2s32s6n3vlrfvd71wu",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-SECONDARYNAMENODE-BASE"
        }
      } ],
      "displayName" : "HDFS",
      "roleConfigGroups" : [ {
        "name" : "hdfs-BALANCER-BASE",
        "displayName" : "Balancer Default Group",
        "roleType" : "BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-1",
        "displayName" : "DataNode Group 1",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2973761536",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-2",
        "displayName" : "DataNode Group 2",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2230321152",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-3",
        "displayName" : "DataNode Group 3",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "892338176",
            "sensitive" : false
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1159725056",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-BASE",
        "displayName" : "DataNode Default Group",
        "roleType" : "DATANODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2579496960",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-BASE",
        "displayName" : "Failover Controller Default Group",
        "roleType" : "FAILOVERCONTROLLER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-BASE",
        "displayName" : "HttpFS Default Group",
        "roleType" : "HTTPFS",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-BASE",
        "displayName" : "JournalNode Default Group",
        "roleType" : "JOURNALNODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-NAMENODE-BASE",
        "displayName" : "NameNode Default Group",
        "roleType" : "NAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022",
            "sensitive" : false
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1715470336",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-BASE",
        "displayName" : "NFS Gateway Default Group",
        "roleType" : "NFSGATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-BASE",
        "displayName" : "SecondaryNameNode Default Group",
        "roleType" : "SECONDARYNAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn",
            "sensitive" : false
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1715470336",
            "sensitive" : false
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ],
    "uuid" : "048f3fd5-64ee-45e3-a324-2828f0236e63"
  } ],
  "hosts" : [ {
    "hostId" : "5571542f-92d1-42e8-99a0-0189f72e83ee",
    "ipAddress" : "172.31.23.7",
    "hostname" : "ip-172-31-23-7.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "888b01fb-fc59-4f20-b5fb-f4a7f1ee3853",
    "ipAddress" : "172.31.27.173",
    "hostname" : "ip-172-31-27-173.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d",
    "ipAddress" : "172.31.30.151",
    "hostname" : "ip-172-31-30-151.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "f73e829a-ab67-4436-9c99-28484e3f9620",
    "ipAddress" : "172.31.31.233",
    "hostname" : "ip-172-31-31-233.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "169d76a2-39be-41a5-8ec3-89678a3f1302",
    "ipAddress" : "172.31.31.49",
    "hostname" : "ip-172-31-31-49.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "151d2c0c71c71ad98943503193b12ac6d7c18874dd4afe10578cd5175d49a740",
    "pwSalt" : 3835632567145019583,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-d3ca5cb9676f8e6f5ba1083fb2cfae89",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "6b91480ca8558bf5457ce20bd928ff2091985cbca06b7ffa366f3290228c0eab",
    "pwSalt" : -6103046279705590523,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "f3536b4995a710d9d6452d2e54a7732a4bc002ae780fc1388d16e09bb065beff",
    "pwSalt" : -2002549912974108733,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-d3ca5cb9676f8e6f5ba1083fb2cfae89",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "967870b4e094fc622280a4f1e4b412449e7436dcf3216161419c71195e4e53df",
    "pwSalt" : 3062101521491076831,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "49966e1f1bee459e78050fc219e5fbd41a9530276957bf1c4cf5273caf9e4740",
    "pwSalt" : -6378820878202397657,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170811-0014",
    "gitHash" : "3c3ea33a12076fb83a8f11c4452c52fac685d01b",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5krqki3f6b57jjtdayk48s01m",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2wg0lbe8advyhi5kbk2mnrp34",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-d3ca5cb9676f8e6f5ba1083fb2cfae89",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "39ocw7x1xzt51snleqjk3exbu",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-d3ca5cb9676f8e6f5ba1083fb2cfae89",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3ayt1ndm0trsh44lub123x7q7",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-d3ca5cb9676f8e6f5ba1083fb2cfae89",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "4eb63078-8e1d-4f18-9631-f0b07781229d"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5ruh8atc2mhevyk9h873a5mmo",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-SERVICEMONITOR-BASE"
      }
    } ],
    "displayName" : "Cloudera Management Service",
    "roleConfigGroups" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-BASE",
      "displayName" : "Activity Monitor Default Group",
      "roleType" : "ACTIVITYMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-BASE",
      "displayName" : "Alert Publisher Default Group",
      "roleType" : "ALERTPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-BASE",
      "displayName" : "Event Server Default Group",
      "roleType" : "EVENTSERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "892338176",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-BASE",
      "displayName" : "Host Monitor Default Group",
      "roleType" : "HOSTMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "892338176",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1159725056",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATOR-BASE",
      "displayName" : "Navigator Audit Server Default Group",
      "roleType" : "NAVIGATOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-NAVIGATORMETASERVER-BASE",
      "displayName" : "Navigator Metadata Server Default Group",
      "roleType" : "NAVIGATORMETASERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-BASE",
      "displayName" : "Reports Manager Default Group",
      "roleType" : "REPORTSMANAGER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-31-49.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password",
          "sensitive" : true
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman",
          "sensitive" : false
        }, {
          "name" : "headlamp_heapsize",
          "value" : "892338176",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-BASE",
      "displayName" : "Service Monitor Default Group",
      "roleType" : "SERVICEMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "892338176",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1159725056",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-TELEMETRYPUBLISHER-BASE",
      "displayName" : "Telemetry Publisher Default Group",
      "roleType" : "TELEMETRYPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/26/2012 8:30",
      "sensitive" : false
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD",
      "sensitive" : false
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh5/parcels/5.8,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/",
      "sensitive" : false
    } ]
  },
  "allHostsConfig" : {
    "items" : [ ]
  },
  "peers" : [ ],
  "hostTemplates" : {
    "items" : [ ]
  }
```
