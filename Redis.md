##  初识 Redis

Redis 是一种 *NoSql* 数据库，其是单线程架构，数据存储在内存中，且提供 *String、list、hash、zset、set* 基本数据结构。

---

## Redis 的启动

Redis 启动分为三种：默认配置启动(`redis-server`)、运行配置启动(`redis-server --configName configValue`)、配置文件启动

Redis 客户端启动方式：`redis-cli -h 127.0.0.1 -p 6370`

Redis 服务关闭：`redis-cli shutdown`

## Redis 通用命令

1. 获取所有键：`keys *`
2. 获取键个数：`dbsize`
3. 判断键是否存在：`exists keyName`
4. 删除键：`del keyName`
5. 设置过期时间：`expire keyName time`
6. 查看剩余时间：`ttl keyName`
7. 查看类型：`type keyName`

## Redis 基本数据结构

### String

1. 设置值：`set key value`
2. 获得值：`get key`
3. 键不存在才设置成功：`setnx key value`
4. 键存在才设置成功：`setxx key value`
5. 批量设置或获取：`mset key value、mget key`
6. 自增：`incr key`