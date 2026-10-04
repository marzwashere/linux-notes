# Linux `grep` Command Guide

## Overview
`grep` is a powerful command-line utility used to search plain-text data sets for lines matching a specific regular expression or search string. It is an essential tool for system administrators reviewing log files.

---

## 1. Basic Keyword Search
To isolate specific entries (such as errors) from a log file:
```bash
grep "ERROR" app.log

grep -i "warning" app.log

# Linux `grep` Command Guide

## Overview
`grep` is a powerful command-line text search utility used to find lines matching a specified pattern in files. It is an essential tool for parsing logs and troubleshooting system issues.

---

## 1. Basic Keyword Search
To isolate specific entries (such as errors) from a log file:
```bash
grep "ERROR" test.log
