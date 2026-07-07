# Task 5 - Capture and Analyze Network Traffic Using Wireshark

## Student Information

| Field | Details |
|--------|---------|
| **Name** | PRASIDDHA PAL |
| **Branch** | CSE (2027) |
| **Internship** | Cyber Security Internship |
| **Task** | Task 5 - Capture and Analyze Network Traffic Using Wireshark |
| **Tool Used** | Wireshark 4.x |
| **Operating System** | Kali Linux |
| **Status** | ✅ Completed |

---

## Objective

Capture live network traffic using Wireshark, identify commonly used network protocols, analyze packet details, and understand network communication.

---

## Tools Used

- Ubuntu Linux
- Wireshark
- Internet Browser
- Terminal

---

## Procedure

1. Installed and launched Wireshark.
2. Selected the active network interface.
3. Started packet capture.
4. Generated network traffic by browsing websites.
5. Stopped the capture after sufficient packets were collected.
6. Applied protocol filters.
7. Analyzed captured packets.
8. Exported the capture as a `.pcapng` file.

---

## Protocols Identified

- DNS
- TCP
- HTTP
- HTTPS/TLS
- ICMP

---

## Packet Analysis

### DNS
- Observed DNS query and response packets.
- Resolved domain names into IP addresses.

### TCP
- Verified TCP Three-Way Handshake.
- Identified SYN, SYN-ACK, and ACK packets.

### HTTP
- Captured HTTP GET requests.
- Observed HTTP 200 OK responses.

### HTTPS/TLS
- Observed TLS Client Hello.
- Server Hello
- Certificate Exchange
- Encrypted communication.

### Follow TCP Stream

- Inspected complete client-server communication.

---

## Learning Outcomes

- Learned how packet capturing works.
- Understood network protocols.
- Practiced filtering packets.
- Analyzed TCP communication.
- Examined encrypted HTTPS traffic.

---

## Repository Structure

```text
wireshark-network-analysis/
├── README.md
├── report/
│   └── PRASIDDHA_Wireshark.pdf
├── capture/
│   └── network_capture.pcapng
└── screenshots/
    ├── 01-home.png
    ├── 02-dns-analysis.png
    ├── 03-tcp-handshake.png
    ├── 04-http-analysis.png
    ├── 05-https-analysis.png
    └── 06-follow-tcp-stream.png
```

---

## Author

**PRASIDDHA PAL**

Cyber Security Internship 

Status: ✅ Completed
