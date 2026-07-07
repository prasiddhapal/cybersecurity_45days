# Task 4: Setup and Use a Firewall on Linux (UFW)

## Student Information

| Field | Details |
|-------|---------|
| **Name** | Your Name |
| **Status** | Completed |
| **Course** | Cyber Security Internship |
| **Task** | Task 4 - Setup and Use a Firewall on Windows/Linux |
| **Operating System** | Ubuntu Linux |
| **Firewall Tool** | UFW (Uncomplicated Firewall) |
| **Date** | DD/MM/YYYY |
| **GitHub** | https://github.com/your-username/firewall-task |

---

## Objective

Configure and test basic firewall rules to allow or block network traffic using UFW.

---

## Environment

- **Operating System:** Ubuntu Linux
- **Firewall:** UFW (Uncomplicated Firewall)
- **Terminal:** Bash

---

## Commands Used

### Check Firewall Status

```bash
sudo ufw status verbose
```

### List Firewall Rules

```bash
sudo ufw status numbered
```

### Block Telnet Port (23)

```bash
sudo ufw deny 23/tcp
```

### Allow SSH Port (22)

```bash
sudo ufw allow 22/tcp
```

### Remove Test Rule

```bash
sudo ufw delete deny 23/tcp
```

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| 01-ufw-status.png | UFW status before configuration |
| 02-firewall-rules.png | Current firewall rules |
| 03-block-port23.png | Blocking TCP port 23 |
| 04-allow-ssh.png | Allowing SSH (Port 22) |
| 05-final-status.png | Final firewall configuration |

---

## Results

- Successfully enabled and verified UFW.
- Listed firewall rules.
- Blocked inbound traffic on TCP port 23.
- Allowed inbound SSH traffic on TCP port 22.
- Removed the temporary block rule.
- Verified firewall configuration after testing.

---

## Key Learnings

- UFW simplifies Linux firewall management.
- Firewall rules control incoming and outgoing network traffic.
- Blocking unused ports improves system security.
- SSH access can be safely allowed while restricting unnecessary services.

---

## Repository Structure

```text
firewall-task/
├── README.md
└── screenshots/
    ├── 01-ufw-status.png
    ├── 02-firewall-rules.png
    ├── 03-block-port23.png
    ├── 04-allow-ssh.png
    └── 05-final-status.png
```

---

## Author

**Name:** Your Name

**GitHub:** https://github.com/your-username

**Status:** ✅ Task Completed Successfully
