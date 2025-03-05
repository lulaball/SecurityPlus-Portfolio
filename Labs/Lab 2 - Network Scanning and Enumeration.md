# Lab 2 - Network Scanning and Enumeration

## Objective
The goal of this lab is to practice using tools to scan networks and enumerate devices. This is a critical skill for understanding how attackers gather information, and how defenders can detect unauthorized scanning activity.

---

## Tools Used
- **Nmap** (Network Mapper)
- **Zenmap** (Nmap GUI - Optional)
- **ipconfig / ifconfig** (to find your IP address)
- **Ping** (basic network discovery)

---

## Steps Performed
### 1. Identify your own IP Address
- Used `ipconfig` (Windows) or `ifconfig` (Linux/Mac) to find your system's IP address.

### 2. Ping Sweep the Network
- Performed a ping sweep using Nmap:  
    ```
    nmap -sn 192.168.1.0/24
    ```
- This identified live hosts on the network.

### 3. Perform a Service Scan
- Used Nmap to detect open ports and services on a target machine:  
    ```
    nmap -sV 192.168.1.10
    ```

### 4. Perform OS Detection
- Ran:  
    ```
    nmap -O 192.168.1.10
    ```

---

## Skills Learned
- Network Discovery Techniques
- Service Detection and Version Scanning
- Operating System Fingerprinting
- Understanding the importance of limiting unnecessary services

---

## Reflection
This lab helped me understand the importance of regularly scanning your own network to detect unauthorized devices or services. Enumeration is a double-edged sword — both attackers and defenders use it. Security teams should be familiar with these techniques to better defend against them.

---

## Screenshots
*(This section is where you can paste any screenshots you took during the lab, such as your Nmap scan results.)*

