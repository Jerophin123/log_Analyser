# Log Analyser

## Overview
**Log Analyser** is a Python-based tool designed to process and analyze server log files. It extracts critical information such as the number of requests per IP address, the most accessed endpoint, and suspicious activities like failed login attempts. The results are neatly summarized in a CSV file for further inspection.

## Features
- **Requests per IP Address**: Counts and reports the number of requests made by each IP address.
- **Most Accessed Endpoint**: Identifies the endpoint that received the highest number of requests.
- **Suspicious Activity Detection**: Tracks IP addresses with failed login attempts (HTTP status code `401`).

## Requirements
- Python 3.6 or later
- `re` (Regular Expression module, included in Python standard library)
- `csv` (CSV handling module, included in Python standard library)
- `collections` (Included in Python standard library)

## Installation
1. Clone the repository or download the script:
   ```bash
   git clone https://github.com/your-username/Log_analyser.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Log_analyser
   ```

## Usage
1. Place your log file in the project directory. Ensure the log file follows a standard format like Apache or NGINX logs.
2. Update the `log_file` variable in the script with the name of your log file:
   ```python
   log_file = "sample.log"
   ```
3. Run the script:
   ```bash
   python log_analyser.py
   ```
4. The results will be saved in a CSV file named `log_analysis_results.csv` in the same directory.

## Output
The output CSV file contains the following sections:
1. **Requests per IP**: A breakdown of the number of requests made by each IP address.
2. **Most Accessed Endpoint**: The endpoint with the highest number of accesses.
3. **Suspicious Activity**: A list of IP addresses with failed login attempts.

## Example
Sample log entry:
```
192.168.1.1 - - [10/Nov/2024:13:55:36 +0000] "GET /index.html HTTP/1.1" 200 1024
```

Result in the CSV:
- **Requests per IP**: 
  ```
  IP Address, Request Count
  192.168.1.1, 10
  ```
- **Most Accessed Endpoint**:
  ```
  Endpoint, Access Count
  /index.html, 50
  ```
- **Suspicious Activity**:
  ```
  IP Address, Failed Login Count
  192.168.1.2, 3
  ```


## Contact
For any questions or feedback, please reach out:
- **Email**: jerophinstanley47@gmail.com
- **GitHub**: [Jerophin](https://github.com/Jerophin)

