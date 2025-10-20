# Tripwire Directory Integrity Script in Linux (Fedora)

This project implements a simple, Python-based directory integrity checker ("tripwire"), which records or audits the hash states of files in a monitored directory.

## 🚩 Project Scenario

You are tasked with building a "tripwire" script to detect added, changed, or removed files by comparing a directory's state against a pre-existing record.

## 📝 Features

- Create a static record of all files in a directory with their hash values.
- Later, audit the directory for changes (modifications, additions, deletions).
- Console reporting for real-time monitoring.
- Error handling for arguments and file operations.

## ⚙️ Usage
- To create a reference record for a directory (in my case, the script runs as 'python3 tripwire.py <directory_to_monitor> <tripwire_record_file> c')
  - The script will evaluate a directory and calculate an MD5 hash value for each file in the directory. I created test files to demonstrate as an example.
  - The 'c' flag simply indicates to create the tripwire record file. 
  - Next, the script will create a tripwire record file to store the file name and hash values. 
- Integrity check for changes (added/removed/modified) in the directory:
  - 'python3 tripwire.py <tripwire_record_file>'
  - This script will evaluate the tripwire record file for any changes to the directory and modifications to files.

## 💡 Key Concepts Demonstrated

- File I/O and directory traversal in Python.
- Cryptographic hash (MD5 or SHA family) for file integrity.
- Command-line argument parsing.
- Data structures for tracking added, removed, modified files.
- Error handling for real-world scripting.

## 📝 Pseudocode & Function Overview
Block comment at the top of `tripwire.py` should provide high-level pseudocode for clarity.

---

## Screenshots:
- Here is my file structure in my home directory, with my tripwire Python file and tripwireDir directory created.
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/8f6c6735-d5e2-45c3-8e7b-2fb31fdb5db4" />
- Brief display of my Python code:
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/55fc449f-d345-4bd3-9303-df29cf240315" />
- Create a sample file in the directory. We will also create a second file to demonstrate a removed file was evaluted in the "compare" script
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/f8cf6a91-a5df-4b3c-9b99-e19be0136f7c" />
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/69434b20-beff-4c2a-8663-ca4ec77e83fa" />
- Demonstration of running "create tripwirerecord" script
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/cfe11fb6-5564-4f80-8392-02792870b913" />
- Demonstration of modifying text, removing a file, and creating a new file
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/ae6f334a-6f17-42c8-8359-3877851c9caf" />
- The "compare" script will evaluate the tripwireRecord file with the directory to assess any files that have been added, removed, or modified.
  - <img width="2568" height="1400" alt="image" src="https://github.com/user-attachments/assets/ec7289ab-722b-4374-a23b-bce121b0fca5" />

I hope this helps you understand how a tripwire code can be greatly beneficial in ensuring file integrity for your systems!

## 🔗 Portfolio

Return to my main portfolio: [JackieG8803 IT Portfolio](https://github.com/JackieG8803)

---

Let me know if you want a sample Python starter code for `tripwire.py`, or help filling in any section!
[tripwire.py](https://github.com/user-attachments/files/23006465/tripwire.py)
