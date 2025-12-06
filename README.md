# 🐧 Linux File Permissions Audit – Access Control & chmod

## 📌 Overview
This project focuses on analyzing, correcting, and securing **Linux file and directory permissions** within a research team’s project directory.  
Using tools such as **ls -la**, **chmod**, and permission string analysis, I identified improper access settings and updated them to align with organizational security policies.

The work demonstrates hands-on experience with Linux permissions, least privilege, hidden files, and secure access control—critical skills for security and IT roles.

---

## 🗂️ Project File

- **Linux-File-Permissions-Audit.pdf**  
  Includes:
  - Permission audit of the *projects* directory  
  - Explanation of Linux permission strings  
  - Corrections to file and directory privileges  
  - Updates to hidden and archived files  
  - Enforcement of least privilege on the `drafts` directory  
  - Verification via `ls -la` command outputs  
  - Screenshots of terminal commands  
  (Full PDF included in this repository)

---

## 🔍 Scenario Summary

According to the PDF (pages 1–5), several security misconfigurations were found:

- A hidden file (`.project_x.txt`) required stricter read-only access  
- A file (`project_k.txt`) incorrectly allowed **write access for others**  
- A directory (`drafts`) allowed group execute permissions, violating the access policy  
- Multiple project files had group permissions misaligned with team requirements  

To address these issues:

### ✔ Initial Audit  
Used: `ls -la`

to list hidden files, subdirectories, and 10-character permission strings.

### ✔ Understanding Permission Strings  
Each file’s string (e.g., `drwxr-xr-x` or `-rw-rw-r--`) was interpreted to determine:

- File type  
- Owner permissions  
- Group permissions  
- Others’ permissions  

### ✔ Correcting File Permissions  
Examples of commands used:

- chmod o-w project_k.txt
- chmod u-w,g-w,g+r .project_x.txt
- chmod g-x drafts


### ✔ Verification  
Re-ran: `ls -la`

to confirm updated permissions were applied correctly.

---

## 🛠️ Skills Demonstrated

- Linux file system navigation  
- Interpretation of permission strings (drwx…, -rw-…)  
- Use of `chmod` for secure access control  
- Managing hidden files and archival policies  
- Enforcing least privilege  
- Identifying permission misconfigurations  
- Command-line verification with `ls -la`  

---

## 🧩 Key Technical Concepts

### **📁 Linux Permission String Breakdown**
As described in the PDF:
- Character 1 → file/directory  
- Characters 2–4 → owner permissions (r, w, x)  
- Characters 5–7 → group permissions  
- Characters 8–10 → others’ permissions  

### **🔐 Least Privilege Enforcement**
Examples include:
- Removing write access for “others”  
- Restricting execute access to a single authorized user  
- Ensuring archived files are read-only for all users except allowed viewers  

---

## 📌 What This Project Shows Employers

This project demonstrates my ability to:

- Audit and correct **Linux file & directory permissions**
- Apply **least privilege** access control  
- Use `chmod`, `ls -la`, and permission strings effectively  
- Work with hidden files, directories, and archival restrictions  
- Identify and fix security misconfigurations  
- Document technical steps clearly using terminal output and screenshots  

---

## 📌 Roles This Project Aligns With

Skills in this project align with responsibilities in:

- **Cybersecurity Analyst (Entry Level)**
- **SOC Analyst – Tier 1**
- **IT Support / Help Desk**
- **Linux System Administrator (Junior)**
- **GRC Analyst (technical controls focus)**

---

## 📬 Contact

- **GitHub Portfolio:** *https://github.com/michaelhanna97*  
- **LinkedIn:** *your LinkedIn link (optional)*  



