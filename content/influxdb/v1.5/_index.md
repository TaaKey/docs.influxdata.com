---
title: InfluxDB 1.5 documentation

menu:
  influxdb:
    name: v1.5
    identifier: influxdb_1_5
    weight: 1
---

InfluxDB is a [time series database](https://www.influxdata.com/time-series-database/) designed to handle high write and query loads.
It is an integral component of the
[TICK stack](https://influxdata.com/time-series-platform/).
InfluxDB is meant to be used as a backing store for any use case involving large amounts of timestamped data, including DevOps monitoring, application metrics, IoT sensor data, and real-time analytics.

InfluxDB 是一个用于处理高写入和查询负载的时间序列数据库，它是Influxdata平台TICK中的一个组成部分。
InfluxDB 是用于处理含有大量的时间戳数据的业务场景（包括DevOps监测，应用指标，物联网传感器的数据，以及实时分析等等）的数据后台存储。

## Key features
## 重要特性

Here are some of the features that InfluxDB currently supports that make it a great choice for working with time series data.
对于下面这些特点的支持，使得 InfluxDB 成为了当前处理时间序列数据的一个很好的选择。

* Custom high performance datastore written specifically for time series data.
The TSM engine allows for high ingest speed and data compression
* Written entirely in Go.
It compiles into a single binary with no external dependencies.
* Simple, high performing write and query HTTP APIs.
* Plugins support for other data ingestion protocols such as Graphite, collectd, and OpenTSDB.
* Expressive SQL-like query language tailored to easily query aggregated data.
* Tags allow series to be indexed for fast and efficient queries.
* Retention policies efficiently auto-expire stale data.
* Continuous queries automatically compute aggregate data to make frequent queries more efficient.

* 专门针对时间序列数据的写入操作定制的高性能数据存储。
TSM引擎允许高摄取速度和数据压缩

* 完全采用 Go语言 实现。
它编译成一个没有外部依赖关系的独立的二进制文件。

* 简单、高性能的编写和查询HTTP API。

* 插件支持其他数据摄取协议如石墨、搜集和opentsdb。

* 适于查询聚合数据的表达式SQL查询语言。

* 标签允许对快速查询和有效查询进行索引。

* 保留策略有效地自动过期数据。

* 连续查询自动计算聚合数据，使频繁查询更高效。

The open source edition of InfluxDB runs on a single node.
If you require high availability to eliminate a single point of failure, consider the [InfluxDB Enterprise Edition](https://docs.influxdata.com/influxdb/v1.5/high_availability/).

当前，开源版本的 InfluxDB 仅支持单节点模式；如若需要高可用版(即多节点的集群版)，请考虑 [InfluxDB企业版](https://docs.influxdata.com/influxdb/v1.5/high_availability/).
