# OSS Audit Project – Shell Scripting Portfolio

## Student Details

* **Name:** Tejas Santosh Paithankar
* **Roll Number:** 24BCY10104
* **Course:** Open Source Software (OSS)
* **Faculty:** Dr. Vikas Panthi
* **Semester:** Winter 2026

---

## Chosen Software

* **Platform:** Linux (GNU/Linux Environment)
* **Shell:** Bash (Bourne Again Shell)
* **Purpose:**
  This project demonstrates the power of Linux and Bash scripting for **system auditing, automation, and monitoring**. The scripts leverage core Linux utilities and reflect open-source principles such as transparency, automation, and efficiency.

---

## Project Overview

This repository contains **5 Bash scripts** designed to automate system inspection, package verification, security auditing, log analysis, and manifesto generation.

---

## Dependencies Required

Ensure the following tools are installed on your Linux system:

* `bash`
* `coreutils` (includes `ls`, `du`, `date`, etc.)
* `grep`
* `awk`
* `dpkg` (for Debian-based systems like Ubuntu/Kali)
* `uname`
* `whoami`

Install dependencies (if needed):

```bash
sudo apt update
sudo apt install coreutils grep awk dpkg
```

---

## Scripts Description

### Script 1: System Identity Report (`system_report.sh`)

**Purpose:**
Displays system information such as kernel version, distribution, user, uptime, and date.

**Key Features:**

* Uses command substitution `$(...)`
* Extracts system metadata
* Generates formatted report

---

### Script 2: Package Inspector (`package_inspector.sh`)

**Purpose:**
Checks if the current kernel package is installed and prints its philosophical significance.

**Key Features:**

* Uses `if-else` for package verification
* Uses `case` statements for classification
* Demonstrates FOSS philosophy mapping

---

### Script 3: Disk & Permission Auditor (`disk_permission_audit.sh`)

**Purpose:**
Audits critical system directories for permissions and disk usage.

**Key Features:**

* Iterates using `for loop`
* Uses `ls -ld` and `du -sh`
* Performs critical check on `/boot/grub`

---

### Script 4: Log Hunter (`log_hunter.sh`)

**Purpose:**
Analyzes log files for errors or specific keywords.

**Key Features:**

* Accepts user input (log file + keyword)
* Implements retry mechanism (while loop)
* Counts and displays recent log entries

---

### Script 5: Manifesto Generator (`manifesto_generator.sh`)

**Purpose:**
Generates a personalized Open Source manifesto file.

**Key Features:**

* Takes user input via `read`
* Creates timestamped file
* Stores structured output

---

## How to Run Scripts (Step-by-Step on Linux)

### Step 1: Clone or Copy Files

```bash
git clone <repository_url>
cd <repository_folder>
```

---

### Step 2: Give Execute Permission

```bash
chmod +x *.sh
```

---

### Step 3: Run Each Script

#### Script 1

```bash
./system_report.sh
```

#### Script 2

```bash
./package_inspector.sh
```

#### Script 3

```bash
./disk_permission_audit.sh
```

#### Script 4

```bash
./log_hunter.sh <logfile> [keyword]
```

Example:

```bash
./log_hunter.sh /var/log/syslog ERROR
```

#### Script 5

```bash
./manifesto_generator.sh
```

---

## Key Learning Outcomes

* Understanding Linux system internals
* Automating administrative tasks using Bash
* Applying control structures (loops, conditions)
* Working with system logs and permissions
* Practicing open-source philosophy through scripting

---

## Notes

* Script 2 works best on **Debian-based systems** (uses `dpkg`)
* Script 4 requires a valid log file path
* Script 5 generates output file:

  ```
  manifesto_<username>.txt
  ```

---

## References

* GNU Project – Free Software Definition
* Open Source Initiative
* *The Cathedral and the Bazaar* – Eric S. Raymond
* *The Linux Command Line* – William Shotts

---

## Conclusion

This project showcases how Linux and Bash scripting can be used for **efficient system auditing and automation**, reflecting the true power of open-source software.

---
