---
title: TiDB Operator 1.1.11 Release Notes
---

# TiDB Operator 1.1.11 Release Notes

Release date: February 26, 2021

TiDB Operator version: 1.1.11

## New Features

- Tune LeaderElection, support user configuration about LeaderElection ([#3794](https://github.com/pingcap/tidb-operator/pull/3794), [@july2993](https://github.com/july2993))
- Add `tidb_cluster` label for the scrape jobs in TidbMonitor to support multiple clusters monitoring ([#3750](https://github.com/pingcap/tidb-operator/pull/3750), [@mikechengwei](https://github.com/mikechengwei))
- Support setting customized store labels according to the node labels ([#3784](https://github.com/pingcap/tidb-operator/pull/3784), [@L3T](https://github.com/L3T))

## Improvements

- Add TiFlash rolling upgrade logic to avoid all TiFlash stores unavailable during upgrade ([#3789](https://github.com/pingcap/tidb-operator/pull/3789), [@handlerww](https://github.com/handlerww))
- Retrieve the region leader count from TiKV Pod directly instead of from PD to get the accurate count ([#3801](https://github.com/pingcap/tidb-operator/pull/3801), [@DanielZhangQD](https://github.com/DanielZhangQD))
- Print RocksDB and Raft log to stdout to support them be collected and queried in the grafana ([#3768](https://github.com/pingcap/tidb-operator/pull/3768), [@baurine](https://github.com/baurine))

## Bug Fixes

- Add blank in backup manager script to avoid the script crashed in some shell ([#3809](https://github.com/pingcap/tidb-operator/pull/3809), [@handlerww](https://github.com/handlerww))