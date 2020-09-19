## 相关概念
**Redis**是完全开源免费的，遵守BSD协议，是一个高性能的**key-value**数据库。

Redis与其他key-value缓存产品相比:支持数据的**持久化，多数据结构**list，set，zset，hash等的存储，支持**数据备份**。

## Redis特点
* 高性能、可持久化
* key-value结构，支持多种数据类型
* **支持事务，数据的原子性(要么不做/全做)**

## Redis应用场景
* 缓存(读写性能优异)
* 计数与消息系统(高并发、发布/订阅阻塞队列功能)
* **分布式会话session与分布式锁(秒杀)**

## Redis vs Mongo
* 存储方式不一样:key-value vs Document
* 使用方式与可靠性不一样:MongoDB SQL 与 ACID 支持
* **应用场景不一样:高性能缓存 vs 海量数据分析**