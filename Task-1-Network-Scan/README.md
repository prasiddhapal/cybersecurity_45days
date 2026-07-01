# 🔍 Task 1: Scan Your Local Network for Open Ports

## 📌 Objective

The objective of this task is to identify open TCP ports on a target host using **Nmap**. This helps understand network reconnaissance, service discovery, and potential security risks associated with exposed services.

---

# 🛠️ Tools Used

- Nmap 7.98
- Linux Terminal
- GitHub

---

# 🎯 Target

**Target Host:** `IP`

---

# 🚀 Command Used

```bash
nmap -sS IP -oN nmap_scan.txt
```

## Command Explanation

| Command | Description |
|---------|-------------|
| `nmap` | Launches the Network Mapper tool. |
| `-sS` | Performs a TCP SYN (Half-Open) Scan to identify open TCP ports. |
| `IP` | Target host to be scanned (actual IP/domain hidden for privacy). |
| `-oN` | Saves the scan results in Normal (text) format. |
| `nmap_scan.txt` | Output file containing the scan results. |

---

# 📊 Scan Result

```
Starting Nmap 7.98

Host is up (0.036s latency).

Not shown: 998 filtered tcp ports (no-response)

PORT    STATE SERVICE
80/tcp  open  http
443/tcp open  https

Nmap done: 1 IP address (1 host up) scanned in 6.68 seconds
```

---

# 📋 Scan Summary

| Target | Host Status | Open Ports | Services |
|---------|------------|------------|-----------|
| IP | Up | 80/tcp, 443/tcp | HTTP, HTTPS |

---

# 🔍 Port Analysis

| Port | Service | Description | Security Consideration |
|------|----------|-------------|------------------------|
| 80/tcp | HTTP | Web server running over an unencrypted connection. | Traffic can be intercepted if HTTPS is not enforced. |
| 443/tcp | HTTPS | Secure web server using SSL/TLS encryption. | Certificates should be valid and the server should use secure TLS configurations. |

---

# ⚠️ Observations

- The target host is reachable.
- A total of **998 TCP ports** are filtered (no response).
- Only **Port 80 (HTTP)** and **Port 443 (HTTPS)** are open.
- The filtered ports may be protected by a firewall or packet filtering rules.

---

# 🔐 Security Recommendations

- Redirect all HTTP traffic to HTTPS.
- Keep the web server software updated.
- Configure a firewall to allow only required services.
- Disable unnecessary services and close unused ports.
- Regularly monitor open ports for unauthorized changes.

---

# 📁 Repository Structure

```
Task-1-Network-Scan/
│
├── README.md
├── nmap_scan.txt
└── screenshots/
    ├── command.png
    └── scan_result.png
```

---

# 📸 Screenshots

## Command Executed

<img width="936" height="328" alt="Screenshot From 2026-06-30 10-37-24" src="https://github.com/user-attachments/assets/2505f2b8-21f2-416f-a345-430a59bda841" />


---

# 📖 Learning Outcomes

During this task, I learned how to:

- Install and use Nmap.
- Perform a TCP SYN Scan (`-sS`).
- Save scan results using the `-oN` option.
- Identify open TCP ports on a target host.
- Interpret Nmap scan output.
- Understand the purpose of common web service ports.
- Document cybersecurity tasks using GitHub.

---

# ✅ Conclusion

The scan successfully identified the target host as active with **two open TCP ports (80 and 443)** corresponding to **HTTP** and **HTTPS** services. Most other ports were filtered, indicating the presence of firewall rules or packet filtering. This exercise provided practical experience in network reconnaissance, service identification, and documenting scan results using GitHub.

---

## 👨‍💻 Author

**Name:** *PRASIDDHA PAL*

**Internship:** Cyber Security Internship

**Tool Used:** Nmap 7.98
