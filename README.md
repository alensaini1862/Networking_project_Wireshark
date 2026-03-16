# SOC Project – Network Traffic Analysis using Wireshark

## 📌 Project Overview

This project demonstrates how  analyst can use Wireshark to capture and analyze network traffic in order to identify potential security issues.

The objective was to monitor login traffic from a vulnerable web application and analyze packets to detect exposed credentials transmitted over an insecure protocol.

---

## 🎯 Project Goals

* Capture network packets using Wireshark
* Analyze HTTP login traffic
* Identify sensitive data transmitted in clear text
* Demonstrate why unencrypted protocols are insecure

---

## 🛠 Tools & Technologies

* Wireshark
* Kali Linux / Windows
* Web Browser
* Vulnerable Test Environment

---

## 🌐 Target Application

Testing was performed on the intentionally vulnerable website:

http://testfire.net

This website is designed for **security testing and training purposes**.

---

## 🔎 Analysis Process

### 1️⃣ Start Packet Capture

Wireshark was started to monitor network traffic on the active network interface.

### 2️⃣ Generate Traffic

A login attempt was performed on the test website using a **dummy username and password**.

### 3️⃣ Apply Filters

To locate relevant packets, the following Wireshark filters were applied:

Example filters:

tcp.port == 80

http

### 4️⃣ Packet Inspection

The HTTP POST request containing the login credentials was analyzed within the captured packets.

---

## 📊 Findings

During packet inspection, the login credentials were visible in the HTTP request because the traffic was transmitted over **unencrypted HTTP**.

This highlights the importance of using **HTTPS encryption** to protect sensitive data.

---

## 📂 Project Files

* `capture.pcapng` – Packet capture file
* `screenshots/` – Screenshots of Wireshark packet analysis
* `README.md` – Project documentation

If the capture file is larger than GitHub limits, it can be downloaded from the link below:

(Add Google Drive or external download link here)

---

## 🔐 Security Insight

Unencrypted protocols such as HTTP allow attackers to capture sensitive information from network traffic. SOC analysts monitor such traffic patterns to detect potential data exposure risks.

---

## ⚠ Disclaimer

This project was conducted in a **controlled lab environment** for educational and cybersecurity research purposes only.

---

## 👨
