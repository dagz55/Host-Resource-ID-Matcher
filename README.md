# Host Resource ID Matcher

The **Host Resource ID Matcher** is a Python script designed to streamline the process of matching hostnames from a host file to resource IDs in a CSV inventory file. It identifies matches and generates a summary report for easy review.

---

## Features

- Reads a list of hostnames from a user-provided or default `host` file.
- Matches hostnames to resource IDs in a CSV inventory (`linux_vm-inventory.csv`).
- Generates a summary with:
  - Total hostnames in the host file.
  - Hosts with and without matching resource IDs.
  - Detailed output of matches.
- Outputs matched lines to `host_resource_id.txt` for further analysis.
- Debug mode to trace execution.

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/dagz55/host-resource-id-matcher.git
   cd host-resource-id-matcher
