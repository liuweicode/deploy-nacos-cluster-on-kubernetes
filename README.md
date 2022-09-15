# k8s 部署nacos

1. 下载源码 2.1.1 版本

```shell
wget https://github.com/alibaba/nacos/archive/refs/tags/2.1.1.zip
```

2. 创建数据库

```sql
CREATE DATABASE IF NOT EXISTS nacos-dev DEFAULT CHARSET utf8 COLLATE utf8_general_ci;
```

3. 初始化数据库

执行 nacos-2.1.1/distribution/conf/nacos-mysql.sql

4. 部署

```shell
kubectl apply -f nacos.yaml
```



