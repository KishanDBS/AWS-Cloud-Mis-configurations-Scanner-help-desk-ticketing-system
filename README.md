```
   _____        _                 _____                                      
  / ____|      | |               / ____|                                     
 | |     _   _ | |__    ___ _ __| (___    ___  _ __   ___  _ __   ___  _ __  
 | |    | | | || '_ \  / _ \ '__|\___ \  / _ \| '_ \ / _ \| '_ \ / _ \| '_ \ 
 | |____| |_| || |_) ||  __/ |   ____) ||  __/| |_) | (_) | | | | (_) | | | |
  \_____|\__,_||_.__/  \___|_|  |_____/  \___|| .__/ \___/|_| |_|\___/|_| |_|
                                               | |                            
                                               |_|                            
```
```markdown

[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)]()
[![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge)]()
[![Flask](https://img.shields.io/badge/Flask-Backend-black?style=for-the-badge)]()
[![AWS](https://img.shields.io/badge/AWS-Security-orange?style=for-the-badge)]()
[![Git LFS](https://img.shields.io/badge/Git-LFS-lightgrey?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)]()

---

## 🔍 Overview

**Cyber Scanner** is a hybrid security auditing platform that combines:

### ✔️ **AWS Cloud Misconfiguration Scanner**
A Python‑based engine that detects:
- Public S3 buckets  
- Weak IAM policies  
- Exposed security groups  
- EC2 misconfigurations  
- CloudTrail logging gaps  
- Compliance deviations  

### ✔️ **Help Desk Ticketing System**
A Flask‑powered web interface that:
- Logs scanner findings  
- Creates and tracks remediation tickets  
- Stores audit evidence  
- Supports ZIP uploads via Git LFS  
- Provides a clean dashboard for analysts  

This project is designed for **cybersecurity students, cloud auditors, and SOC teams** who need a lightweight but powerful scanning + ticketing workflow.

---

## 🏗️ Architecture

```
                    ┌──────────────────────────┐
                    │   AWS Cloud Environment   │
                    │  (S3, IAM, EC2, SG, CT)   │
                    └─────────────┬────────────┘
                                  │
                                  ▼
                     ┌────────────────────────┐
                     │  Misconfiguration       │
                     │      Scanner            │
                     │  (Python / Boto3)       │
                     └─────────────┬──────────┘
                                   │ Findings
                                   ▼
                     ┌────────────────────────┐
                     │  Help Desk Ticketing    │
                     │   System (Flask UI)     │
                     └─────────────┬──────────┘
                                   │ Tickets
                                   ▼
                     ┌────────────────────────┐
                     │   SQLite / MySQL DB     │
                     │  (Evidence + Reports)   │
                     └────────────────────────┘
```

---

## 📂 Project Structure

```
/scanner
    aws_scanner.py
    utils/
    reports/

/helpdesk
    app.py
    templates/
    static/
    tickets/

/database
    schema.sql
    migrations/

/evidence
    *.zip  (tracked using Git LFS)
```

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/KishanDBS/Cyber-Scanner.git
cd Cyber-Scanner
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## 📦 Git LFS Setup (for ZIP evidence files)

```bash
git lfs install
git lfs track "*.zip"
git add .gitattributes
git add evidence/*.zip
git commit -m "Add evidence ZIP files using Git LFS"
git push origin main
```

---

## ▶️ Running the Scanner

```bash
python scanner/aws_scanner.py
```

---

## ▶️ Running the Help Desk Web App

```bash
cd helpdesk
python app.py
```

App runs at:

```
http://127.0.0.1:5000
```

---

## 🛡️ Security Features

- Audit‑ready evidence generation  
- Cloud misconfiguration reporting  
- Ticket lifecycle tracking  
- Secure client‑server design  
- Optional role‑based access  
- Compliance‑aligned scanning logic  

---

## 🤝 Contributing

Pull requests are welcome.  
For major changes, open an issue to discuss your proposal.

---

## 📄 License
![CS 6](https://github.com/user-attachments/assets/560e174e-1614-40fd-851e-db751504cf73)
![CS 1](https://github.com/user-attachments/assets/45f69d54-2365-43d3-b61f-73d66163df71)
![CS 2](https://github.com/user-attachments/assets/f8ed14e8-17de-47d1-85a5-f86b7fc8e6b0)
![CS 3](https://github.com/user-attachments/assets/29d39562-9cd2-4082-bd51-cca6d9e05217)
![CS 4](https://github.com/user-attachments/assets/710063d4-faa3-42ce-a8c5-557fd46fdc60)
![CS 5](https://github.com/user-attachments/assets/af0a8df7-edf5-48c6-baaa-efc278bbbd4c)


This project is licensed under the **MIT License**.

---


Just tell me what you want next.
