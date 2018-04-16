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

InfluxDB 是一种时间序列数据库(有时也叫做：实时数据库)，其被设计用来处理高写入、查询平衡的业务场景。
它是。
InfluxDB 是用来处理任何含有大量的时间戳数据的后台保存，包括 DevOps监控、应用程序指标监控、物联网传感器数据、以及实时分析。

## Key features

Here are some of the features that InfluxDB currently supports that make it a great choice for working with time series data.

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

The open source edition of InfluxDB runs on a single node.
If you require high availability to eliminate a single point of failure, consider the [InfluxDB Enterprise Edition](https://docs.influxdata.com/influxdb/v1.5/high_availability/).
