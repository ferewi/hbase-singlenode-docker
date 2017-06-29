### Supported tags and respective ```Dockerfile``` links
* [```1.2.4```,```latest```, (1.2.4/Dockerfile)](https://github.com/jimtonic/hbase-singlenode-docker/blob/1.2.4/Dockerfile)

## How To Use

### 1. Run the image

```
docker run -d --name some_hbase jimtonic/hbase-singlnode
```

Exposed Ports:
* 2181  - HBase's Embedded zookeeper cluster
* 16010 - HBase Master web UI at :16010/master-status;  ZK at :16010/zk.jsp
* 8080  - REST API
* 8085  - REST Web UI at :8085/rest.jsp
* 9090  - Thrift API
* 9095  - Thrift Web UI at :9095/thrift.jsp

### 2. Bind a data directory
```
docker run -d --name some_hbase -v your_local_dir:/data/hbase jimtonic/hbase-singlenode
```

