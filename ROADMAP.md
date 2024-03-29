
Roadmap
=======

General Features
================

- 💤 historical records storage + snapshotting ("3 weeks of data")
- 💤 filtering (both ingress and policy)
- 💤 query engine
- 💤 ingress connectors (e.g. Kafka, WebSockets)
- 💤 egress connector for time-series database.

Development per Component
=========================

**`Rotonda-store`**

- ✅ stabilize single-threaded store
- 🦀 stabilize multi-threaded store
- 🦀 stabilize API
- 🦀 robust error handling (get rid of all the unwraps)
- 🦀 benchmarks matrix IPv4/IPv6 `local_array`/`local_vec`
- 🦀 unit tests & acceptance tests matrix
- optimizations: better hashing, cache padding, etc.
- fuzzer IPv4/IPv6

**`Rotonda-runtime`**

- ✅ setup `tokio` skeleton with logging etc.
- keep history window (serials).
- snapshot/restore functionality.
- `systemd` integration.

**`Rotoro`**

- clone RTR and generalize it

**`Rotonda-transformers`**

- build pub/sub unit for BMP ingress

**`Routecore`**

- ✅ prefix types
- ✅ route record example types
- 🦀 BGP/BMP types for parsing
