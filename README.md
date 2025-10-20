# Tripwire Directory Integrity Script

This project implements a simple, Python-based directory integrity checker ("tripwire"), which records or audits the hash states of files in a monitored directory.

## 🚩 Project Scenario

You are tasked with building a "tripwire" script to detect added, changed, or removed files by comparing a directory's state against a pre-existing record.

## 📝 Features

- Create a static record of all files in a directory with their hash values.
- Later, audit the directory for changes (modifications, additions, deletions).
- Console reporting for real-time monitoring.
- Error handling for arguments and file operations.

## ⚙️ Usage


## 📸 Screenshots

Insert screenshots here after running the script:

- ![Creating record demo](screenshots/create_record_demo.png)
- ![Detection run demo](screenshots/detection_demo.png)

## 💡 Key Concepts Demonstrated

- File I/O and directory traversal in Python.
- Cryptographic hash (MD5 or SHA family) for file integrity.
- Command-line argument parsing.
- Data structures for tracking added, removed, modified files.
- Error handling for real-world scripting.

## 📝 Pseudocode & Function Overview
Block comment at the top of `tripwire.py` should provide high-level pseudocode for clarity.

---

## Example Output


## 🔗 Portfolio

Return to my main portfolio: [JackieG8803 IT Portfolio](https://github.com/JackieG8803)

---

Let me know if you want a sample Python starter code for `tripwire.py`, or help filling in any section!
