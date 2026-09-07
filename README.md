# 🧪 Cybersecurity Labs, Notes & Cheat Sheets

Welcome to my personal cybersecurity knowledge base. This repository documents my hands-on learning journey, practical lab exercises, network analysis notes, and technical cheat sheets.

---

### 📌 Repository Overview
- 🐧 **Linux Essentials:** Command-line usage, permissions, and system administration basics.
- 📡 **Networking & Protocols:** OSI layers, TCP/IP, packet analysis, and subnets.
- 🛠️ **Security Tools:** Wireshark, Nmap, and basic network scanning methodologies.
- 📝 **Lab Notes:** Technical writeups and summaries from practical learning modules.

---

### 🐧 Linux Essentials Cheat Sheet

| Command | Description | Example / Usage |
| :--- | :--- | :--- |
| `ls -la` | List all files including hidden ones with detailed permissions | `ls -la /var/log` |
| `chmod` | Change file read/write/execute permissions | `chmod +x script.sh` |
| `grep` | Search for a specific text string inside files | `grep -rn "error" /var/log/` |
| `find` | Find files matching specific search criteria | `find / -name "*.conf" 2>/dev/null` |
| `ss` / `netstat` | Display active network connections and listening ports | `ss -tuln` |
| `ip a` | View network interfaces and assigned IP addresses | `ip a` |

---

### 📡 Networking & Core Protocols

#### Common Security Ports & Services
| Port | Protocol | Service / Purpose |
| :--- | :--- | :--- |
| `21` | TCP | **FTP** (File Transfer Protocol) |
| `22` | TCP | **SSH** (Secure Shell - Encrypted) |
| `53` | UDP/TCP | **DNS** (Domain Name System) |
| `80` | TCP | **HTTP** (Unencrypted Web Traffic) |
| `443` | TCP | **HTTPS** (TLS/SSL Encrypted Web Traffic) |

#### OSI Model Quick Reference
1. **Physical:** Bits, cables, and network hardware signals.
2. **Data Link:** Frames, MAC addresses, and switches.
3. **Network:** Packets, IP addresses, and routers.
4. **Transport:** Segments, TCP/UDP ports, and end-to-end reliability.
5. **Session:** Session management and connection maintenance.
6. **Presentation:** Data encryption, SSL/TLS, and formatting.
7. **Application:** End-user protocols (HTTP, SSH, DNS, FTP).

---

### 🛠️ Basic Security Tools Reference

#### Nmap Scanning Commands
```bash
# Host discovery (Ping scan across local subnet)
nmap -sn 192.168.1.0/24

# Basic TCP port scan
nmap 192.168.1.10

# Service version detection & OS detection
nmap -sV -O 192.168.1.10
