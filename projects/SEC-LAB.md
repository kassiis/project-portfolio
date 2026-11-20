# SEC_LAB Telemetry & Monitoring System

**GitHub Repository:** `kassiis/sec-lab`  
**Source code:** Private repository  
**Project Category:** Cybersecurity & Systems Infrastructure  
**Development Status:** Active / Operational Prototype  

---

## 1. Overview

**SEC_LAB Telemetry** is a lightweight, high-performance system monitoring service and dashboard engineered for cybersecurity laboratory environments. The system couples a zero-dependency Go daemon that gathers kernel-level host metrics with an interactive web dashboard for real-time observability.

---

## 2. Project Purpose

Experimental security testing and malware analysis labs require continuous host observability that does not distort system metrics or introduce external dependency attack vectors. This project delivers:

- A minimal-footprint telemetry collector written purely in standard library Go.
- Non-invasive system metric sampling via direct virtual filesystem parsing.
- In-memory bounded historical buffering with zero disk writes.
- A live web dashboard visualizing host telemetry for lab operators.

---

## 3. Key Capabilities

- **Direct Kernel Telemetry:** Extracts real-time system metrics directly from the Linux `/proc` virtual filesystem:
  - Non-blocking CPU utilization deltas computed from `/proc/stat`.
  - Memory allocation and utilization profiles parsed from `/proc/meminfo`.
  - Cumulative cross-interface network throughput from `/proc/net/dev`.
  - Storage capacity and volume utilization gathered via filesystem syscalls.
- **Bounded In-Memory Time Series:** Custom fixed-capacity circular ring buffer providing $O(1)$ telemetry insertion and automatic oldest-sample eviction with zero runtime heap reallocations.
- **Thread-Safe Concurrency:** Granular read/write synchronization using `sync.RWMutex`, allowing simultaneous background metric acquisition and concurrent HTTP API queries.
- **Portable Cross-Platform Architecture:** Clean build-tag decoupling (`collector_linux.go` vs portable fallback stubs) allowing compilation and local testing across environments.
- **RESTful Telemetry API:** Standards-compliant JSON endpoints supporting temporal queries, sample limits, and RFC3339 timestamp filtering.
- **Interactive Monitoring Dashboard:** Lightweight frontend interface presenting real-time performance indicators and historical trend graphs.

---

## 4. Technologies Used

- **Telemetry Daemon:** Go (Golang) — 100% Standard Library (zero third-party dependencies)
- **Concurrency & Memory:** Go goroutines, channels, and `sync.RWMutex` ring buffers
- **Systems Interface:** Linux `/proc` virtual filesystem, POSIX syscalls
- **Frontend Dashboard:** HTML5, CSS3, JavaScript (ES6+), Charting Engine
- **Testing & Verification:** Go standard `testing` framework (unit coverage across collectors, parsers, and handlers)

---

[← Return to Project Portfolio](../README.md)
