# Day 3: Kali Linux Basics and Windows Hacking

## Introduction

Today's session focused on fundamental commands within the Kali Linux terminal.
## Antivirus Concepts
### Key Antivirus Functions

* **Quarantine Malware:** Antivirus software isolates detected malware to prevent it from infecting or further damaging the system.

# 🔍 Types of Antivirus Analysis

Antivirus software uses two main methods to detect and analyze threats:

---

## 1. 🧊 Static Analysis

- Analyzes files **without executing** them.
- Uses **signature-based** and **heuristic-based** detection.
- **Fast** and **safe**.
- May miss **new, unknown, or obfuscated** threats.

---

## 2. ⚙️ Dynamic Analysis (Runtime Analysis)

- Executes the file in a **controlled environment**.
- Monitors real-time **behavior** (e.g., file modifications, registry access, network activity).
- Effective against **zero-day** and **stealthy malware**.
- **Slower** and uses more resources.

---

## 🧪 Sandbox

- A **secure, isolated environment** used in dynamic analysis.
- Runs suspicious files **safely** without affecting the main system.
- Logs behavior for detailed analysis.
- Commonly used in **cloud-based antivirus systems**.

---

> ⚠️ Summary:  
> - **Static Analysis** = Fast & safe, but may miss new threats.  
> - **Dynamic Analysis** = Detailed & effective, but slower.  
> - **Sandbox** = Safe testing space for running unknown files.


## Kali Linux Terminal Commands
During the class, I explored and executed several basic commands in the Kali Linux terminal the commands which i used are:
| Command       | Uses                                |Images |
| ------------- | ----------------------------------- |-------|
| `ls`          | Lists directory contents            |<img width="805" height="61" alt="image" src="https://github.com/user-attachments/assets/7a7a5e32-6e38-4a03-a937-8ecf342b69e6" />|
| `cd`          | Changes directory                   |<img width="257" height="97" alt="image" src="https://github.com/user-attachments/assets/f2889d76-59bc-48b5-950f-4db2cfddacf5" />|
| `pwd`         | Shows current directory path        |<img width="252" height="60" alt="image" src="https://github.com/user-attachments/assets/eed05587-9c6e-4a1d-9938-1c3d614c3474" />|
| `mkdir`       | Creates a new directory             |<img width="260" height="105" alt="image" src="https://github.com/user-attachments/assets/054001a9-17eb-4258-aa77-eb6321e9b56c" />|
| `rmdir`       | Deletes an empty directory          |<img width="235" height="162" alt="image" src="https://github.com/user-attachments/assets/06090a09-0ad1-46db-9c91-90ccfb0d3458" />|
| `touch`       | Creates a new empty file            |<img width="260" height="115" alt="image" src="https://github.com/user-attachments/assets/6c7831d1-1d23-448b-900b-c260df7e28da" />|
| `man`         | Opens the manual page for a command |<img width="176" height="42" alt="image" src="https://github.com/user-attachments/assets/04c9d7ed-1022-4f87-b857-806a9f63d58d" />|
| `echo`        | Prints a message to terminal        |<img width="193" height="62" alt="image" src="https://github.com/user-attachments/assets/8e226830-3c15-4aa6-8f8e-eaafe4ff54da" />|
| `chmod`       | Changes file permissions            |<img width="396" height="131" alt="image" src="https://github.com/user-attachments/assets/dea146ba-5992-4a18-9c17-d82be1052da6" /> <br>  />|
| `clear`       | Clears terminal screen              |Before:<img width="1048" height="897" alt="image" src="https://github.com/user-attachments/assets/84b275cc-ab8b-44bf-baef-d9404e5860c0" /> After:<img width="1057" height="302" alt="image" src="https://github.com/user-attachments/assets/45a1d878-5970-4c74-9047-44c41338ad4e" />|
| `ls -lh`      |Lists directory contents with detailed information |<img width="403" height="67" alt="image" src="https://github.com/user-attachments/assets/3a47ec66-3361-484f-bf48-c44e6cd1be50" />|

