

# 🚀 Log Analyser

## 📋 Overview
**Log Analyser** is a Python-based tool for processing and analyzing server log files. It extracts critical insights such as:
- Number of requests per IP address.
- The most accessed endpoints.
- Suspicious activities like failed login attempts (HTTP 401).  

The results are neatly summarized in a CSV file for further analysis and reporting, making it an essential tool for web developers, system administrators, and security analysts.

---

## 🌟 Features
| **Feature**                      | **Description**                                                                 |
|-----------------------------------|---------------------------------------------------------------------------------|
| 📊 **Requests per IP Address**       | Counts and reports the number of requests made by each IP address.             |
| 🌐 **Most Accessed Endpoint**        | Identifies the endpoint that received the highest number of requests.           |
| 🔐 **Suspicious Activity Detection** | Tracks IP addresses with failed login attempts (HTTP status code `401`).       |

---

## 🛠️ Requirements
| **Component**       | **Details**                                   |
|----------------------|-----------------------------------------------|
| **Python**           | Version 3.6 or later                        |
| **Modules**          | `re`, `csv`, `collections` (all standard libraries) |

---

## ⚙️ Installation
Follow these simple steps to set up Log Analyser on your system:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Log_analyser.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd Log_analyser
   ```

---

## 🚀 Usage
1. **Prepare the Log File**: Place your log file (e.g., `sample.log`) in the project directory.  
   Ensure the log file adheres to standard formats (e.g., Apache, NGINX).

2. **Update the File Path**: Edit the `log_file` variable in the script with your log file's name:
   ```python
   log_file = "sample.log"
   ```

3. **Run the Script**:  
   Execute the script using Python:
   ```bash
   python log_analyser.py
   ```

4. **Check the Results**:  
   The script generates a CSV file named `log_analysis_results.csv` in the same directory.

---

## 📂 Output Details
The output CSV file contains the following sections:

### 1️⃣ **Requests per IP**
| **IP Address**   | **Request Count** |
|-------------------|-------------------|
| 192.168.1.1       | 10                |
| 203.0.113.12      | 45                |
| 198.51.100.42     | 20                |

### 2️⃣ **Most Accessed Endpoint**
| **Endpoint**      | **Access Count** |
|--------------------|------------------|
| /index.html        | 50               |
| /home              | 30               |
| /contact           | 15               |

### 3️⃣ **Suspicious Activity**
| **IP Address**    | **Failed Login Count** |
|--------------------|------------------------|
| 203.0.113.10      | 3                      |
| 198.51.100.42     | 7                      |

---

## 🖥️ Example
**Sample Log Entry**:  
```
192.168.1.1 - - [10/Nov/2024:13:55:36 +0000] "GET /index.html HTTP/1.1" 200 1024
```

**Result in CSV**:  

- **Requests per IP**:  
  | IP Address     | Request Count |
  |----------------|---------------|
  | 192.168.1.1    | 10            |

- **Most Accessed Endpoint**:  
  | Endpoint       | Access Count  |
  |----------------|---------------|
  | /index.html    | 50            |

- **Suspicious Activity**:  
  | IP Address     | Failed Login Count |
  |----------------|---------------------|
  | 192.168.1.2    | 3                  |

---

## 🔧 Customization
Easily customize Log Analyser to fit your needs:
1. **Input & Output File Paths**:  
   Modify the `log_file` and `output_csv` variables in the script:
   ```python
   log_file = "your_log_file.log"
   output_csv = "your_output_file.csv"
   ```

2. **Regex Pattern**:  
   Adjust the `log_pattern` in the script to parse non-standard log formats.

---

## 💡 Potential Use Cases
| **Use Case**                        | **Description**                                                             |
|-------------------------------------|-----------------------------------------------------------------------------|
| **Web Traffic Analysis**            | Analyze server usage patterns to optimize performance.                      |
| **Security Monitoring**             | Detect potential malicious activities, such as failed login attempts.       |
| **Endpoint Optimization**           | Identify high-traffic areas to improve endpoint performance.                |

---

## 🌟 Why Choose Log Analyser?
Log Analyser is a lightweight, easy-to-use tool that requires no external dependencies. It’s ideal for anyone who wants structured insights from raw server logs in just a few steps.

---

## 📞 Contact

### Name: Jerophin D R
| **Contact Method**       | **Details**                                      |
|---------------------------|-------------------------------------------------|
| ✉️ **Email**                | [jerophinstanley47@gmail.com](mailto:jerophinstanley47@gmail.com) |
| 💻 **GitHub**               | [Jerophin](https://github.com/Jerophin123)         |
| 📱 **Linkedin**               | [Jerophin](https://www.linkedin.com/in/jerophin-d-r-b9a73b257/)         |


Feel free to reach out for questions, suggestions, or feedback! Contributions are always welcome. 😊


