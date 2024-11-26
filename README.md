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

2.	Set up Python Environment
Ensure Python 3.* is installed.

## Usage

1.	Place your host file in the script directory. The file should contain hostnames, one per line.

2.	Place the linux_vm-inventory.csv file in the script directory.

3.	Run the script:
```
    	python host_resource_id_matcher.py
```
4.	Follow prompts to provide the host file name (or press Enter to use host).

5.	Review the generated host_resource_id.txt and summary in the terminal.


## Debug Mode

Could you set the DEBUG variable to True in the script to enable debug mode for detailed output?

Example Output

Terminal Summary:
Summary:
==================================================
Total hostnames in host file: 10
Total resource IDs found: 7
Hosts with matching resource IDs: 7
Hosts with NO matching resource IDs: 3

Hostnames with no matching resource IDs:
--------------------------------------------------
- missing-host1
- missing-host2
- missing-host3

Results have been written to host_resource_id.txt
