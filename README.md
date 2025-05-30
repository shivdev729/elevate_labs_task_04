# 📄 Task 4 of the Elevate Labs Cybersecurity Internship
# Windows Firewall Configuration Configuration and Testing Report

**Target Host:** 192.168.135.40 
**Host OS:** Windows
**Scan Date:** May 27, 2025  

---

## 📄 Listing Current Firewall Rules

### ➤ Method (GUI)

![Firewall rules](https://github.com/shivdev729/elevate_labs_task_04/blob/main/listed%20rules.JPG)

## 📄 Rule for Blocking Port

### ➤ Method (GUI)

![P1](https://github.com/shivdev729/elevate_labs_task_04/blob/main/p1.JPG)
![P2](https://github.com/shivdev729/elevate_labs_task_04/blob/main/p2.JPG)
![P3](https://github.com/shivdev729/elevate_labs_task_04/blob/main/p3.JPG)
![Telnet blocked](https://github.com/shivdev729/elevate_labs_task_04/blob/main/telnet_blocked.JPG)

---

## 📄 Testing Rule

### ➤ Method (GUI)

![P4](https://github.com/shivdev729/elevate_labs_task_04/blob/main/p4.JPG)


---

## 📄 Reverting to original state

### ➤ Method (GUI)

![Original](https://github.com/shivdev729/elevate_labs_task_04/blob/main/original_state.JPG)

---

#  How Firewalls Filter Traffic – Summary

Firewalls act as a **security barrier** between trusted internal networks and untrusted external networks (like the internet). They filter traffic based on a set of **rules** to allow or block data packets.

---

##  Key Filtering Criteria

### 1. **IP Address**
- Filters based on **source** or **destination** IP.
- _Example_: Block traffic from known malicious IPs.

### 2. **Port Number**
- Blocks or allows specific **TCP/UDP ports**.
- _Example_: Block port 23 (Telnet), allow port 80 (HTTP).

### 3. **Protocol**
- Filters by protocol type (e.g., **TCP**, **UDP**, **ICMP**).
- _Example_: Block all incoming ICMP (ping) requests.

### 4. **Direction of Traffic**
- **Inbound**: Traffic entering your system.
- **Outbound**: Traffic leaving your system.

### 5. **Application or Service**
- Some firewalls filter based on the **application** using the network.
- _Example_: Allow traffic for Chrome, block unknown apps.

### 6. **Packet Inspection**
- Advanced firewalls perform **Deep Packet Inspection (DPI)** to analyze packet content.
- Useful for detecting and blocking malware or unauthorized data transfers.

---

## 📋 Types of Rules Used

- **Allow (Permit)** – Let traffic through if it matches the rule.
- **Deny (Block)** – Block traffic that matches the rule.
- **Default Policy** – Typically “deny all unless explicitly allowed.”

---

## How It Works (Flow Overview)

Incoming/Outgoing Traffic → Firewall Rule Set → Decision:
→ Matches an "Allow" Rule → Passes through
→ Matches a "Deny" Rule → Blocked
→ No Match → Default policy applied (usually block)

__Submitted by__:- Shivang Shukla
