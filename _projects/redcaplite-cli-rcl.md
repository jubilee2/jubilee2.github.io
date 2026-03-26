---
title: RedcapLite 2.0 CLI (rcl)
summary: Built the 2.x RedcapLite command-line experience with profile-based access, metadata workflows, and project-to-project metadata sync.
order: 5
tools:
  - Python
  - argparse
  - pandas
  - requests
  - PyYAML
  - keyring
  - REDCap API
home_metrics:
  - Command-first UX with rcl <command> <profile> patterns
  - Profile setup with API validation and secure credential handling
  - Cross-project metadata comparison and optional sync
---

## Overview

Built the **RedcapLite 2.0 CLI** experience as a command-first layer on top of the Python API client, centered on the `rcl` command. The CLI supports profile-based project access, metadata operations, and project-to-project metadata synchronization.

## Why It Matters

REDCap metadata tasks are often repetitive and error-prone, especially across multiple projects and environments. This CLI improves consistency and safety by making key metadata workflows accessible from the terminal with repeatable commands.

## Selected Capabilities

- Designed a command-first structure using `rcl <command> <profile> ...` for scriptable, automation-friendly usage.
- Added interactive profile setup with API URL validation, secure token prompting, and credential storage via OS keyring with local fallback support.
- Built metadata workflows for pull, list, add, edit, and remove operations, including preview/confirm flows before import.
- Added `rcl profiles` for listing saved REDCap connections.
- Added `rcl sync` to compare metadata between two profiles and optionally import changes into the target project.
- Helped organize the CLI into reusable modules for shared client bootstrapping, output helpers, prompts, and registry-driven command routing.

## Tech Stack

- Python
- argparse
- pandas
- requests
- PyYAML
- keyring
- REDCap API

## Links

- GitHub: [https://github.com/jubilee2/RedcapLite](https://github.com/jubilee2/RedcapLite)
- PyPI: [https://pypi.org/project/redcaplite/](https://pypi.org/project/redcaplite/)
