---
title: RedcapLite Python REDCap API Client
summary: Built and maintained a lightweight Python REDCap client package to simplify exports/imports and project administration workflows.
order: 4
tools:
  - REDCap API
  - Python
  - pandas
  - requests
  - PyPI
home_metrics:
  - Reduced REDCap integration boilerplate with reusable endpoint wrappers
  - Added pandas-friendly CSV parsing controls for safer analytics workflows
  - Published reusable package to PyPI with automated test coverage
---

## Overview

**RedcapLite (`redcaplite`)** is a lightweight Python client for working with the REDCap API across data export/import and project administration tasks. It provides a clean interface for common REDCap endpoints and supports pandas-friendly CSV parsing for analytics workflows.

## Why It Matters

- Reduces REDCap API boilerplate in scripts, notebooks, and integration jobs by standardizing request/response handling.
- Improves downstream data handling with pandas CSV parsing controls, including preserving identifier columns as strings.
- Distributed for reuse through PyPI releases with automated testing.

## Selected Capabilities

- Export, import, and delete operations for common REDCap objects (records, metadata, arms, events, DAGs, users, and roles).
- Convenience wrappers for frequent workflows including reports, logs, PDF export, and file operations.
- Pandas-compatible CSV parsing with `pd_read_csv_kwargs` support for explicit dtype control.

## Tech Stack

- Python package (Python >= 3.8)
- requests
- pandas
- MIT License

## Links

- GitHub: [https://github.com/jubilee2/RedcapLite](https://github.com/jubilee2/RedcapLite)
- PyPI: [https://pypi.org/project/redcaplite/](https://pypi.org/project/redcaplite/) (latest: v1.4.2)
