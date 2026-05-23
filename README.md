# Web-Based Digital Forensics Evidence Analyzer 🕵️‍♂️⛓️
### A Full-Stack Blockchain Core Framework for Secure Chain of Custody Management

---

## 📌 Project Overview
This repository contains a full-stack decentralized simulation module that models the internal cryptographic operations of leading blockchain systems (like Bitcoin and Ethereum) to solve a critical issue in modern cybersecurity: **digital evidence tampering**.

Traditional digital evidence management frameworks store sensitive files (like disk raw images, network logs, or system screenshots) in centralized database systems. This creates a single point of failure where unauthorized users or corrupt administrators could modify entries, break the **Chain of Custody**, and render evidence inadmissible in a court of law.

Our solution re-engineers classic **blockchain wallet and transaction dynamics** into an **Evidence Wallet architecture**. By swapping financial transactions for digital evidence metadata and anchoring them with asymmetric signatures, we guarantee an unalterable, transparent history of forensic activity.

---

## 🎓 Academic Context & Project Team
This software was developed as a group-based project milestone at the **University of Wah**.
* **Course Assignment:** Blockchain Architecture & Web Engineering Simulation Prototype
* **Instructor:** Ma'am Muniba Khan
* **Project Team:**
  * **Awais Asif**
  * **Seemab Khan**
  * **Rubaiqa Pervez**

---

## 🛠️ System Architecture & Lab Requirements Mapping

Our platform successfully addresses all 6 mandatory laboratory architectural requirements:

| Lab Checkpoint Requirement | Implementation Mapping in Evidence Console | Technical Backend Mechanism |
| :--- | :--- | :--- |
| **1. Wallet System** | **Investigator Cryptographic Profile** | Pre-configures static keys for node accounts (`Awais`, `Rubaiqa`, `Seemab`). Generates a 32-byte private key and computes a 40-character `0x` public address. |
| **2. Transaction System** | **Evidence Registry Framework** | Captures structured parameters where `Sender` maps to the Officer, `Receiver` maps to the File Object name, and `Amount` maps to the Case Target String. |
| **3. Digital Signature System** | **Cryptographic Tamper Sealing** | Binds the runtime evidence properties directly to the investigator's active secret private key string via a SHA-256 hashing sequence. |
| **4. Verification System** | **Flask Core Verification Gate** | The backend computes `expected_material = f"{record_id}{private_key}"`. If the hash check fails, it triggers an instant alert log; if valid, it accepts the block entry. |
| **5. Blockchain Storage** | **Immutable Forensic Ledger** | Appends valid blocks sequentially inside an explicit list storage layout tracking exact `block_height`, hash timestamps, and custom payload properties. |
| **6. Diffie-Hellman Integration** | **Secure Session Handshake** | Executes modular exponentiation calculations using static prime parameters ($P=23, G=5$) allowing two distinct officers to derive identical matching shared secrets. |

---

## 💻 Technical Stack
* **Frontend Dashboard:** HTML5 / CSS3 / ES6 JavaScript (Enterprise Slate Dark-Theme layout with smooth view-switching viewport logic)
* **Backend API Node:** Python 3 / Flask Microframework & `flask-cors` (Native custom cryptographic algorithms tracking system states)

---

## 🚀 How to Run and Test Locally

Follow these quick steps to get the server running and test the validation pipeline on your machine:

### 1. Clone the Repository
```bash
git clone [https://github.com/rubaiqapervez26/Project_Architecture_demo.git](https://github.com/rubaiqapervez26/Project_Architecture_demo.git)
cd Project_Architecture_demo
