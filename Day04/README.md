
# 🖧 Networking Notes

## 📌 What is a Network?
A **network** is a group of two or more connected computers or devices that can share data, resources, and services.

- **Types**: LAN, WAN, MAN, PAN  
- **Purpose**: File sharing, Internet access, communication, printing, etc.

---

## 📌 What is a Subnet?
A **subnet** (short for "subnetwork") is a logically visible subdivision of an IP network.

- Helps organize and optimize traffic within networks.
- Uses **subnet masks** to divide the IP address.
- Example:  
  IP: `192.168.1.0`  
  Subnet Mask: `255.255.255.0`

---

## 📌 TCP vs UDP – Protocol Comparison

| Feature           | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
|-------------------|-------------------------------------|-------------------------------|
| Connection Type   | Connection-oriented                 | Connectionless                |
| Reliability       | High – guaranteed delivery          | Low – no guarantee            |
| Speed             | Slower                              | Faster                        |
| Use Cases         | HTTP, FTP, Email                    | DNS, Video Streaming, VoIP    |
| Error Checking    | Yes                                 | Minimal                       |
| Packet Order      | Maintains order                     | No order guarantee            |

---

## 📌 IPv4 vs IPv6

| Feature         | IPv4                                | IPv6                                  |
|-----------------|--------------------------------------|----------------------------------------|
| Address Length  | 32-bit (e.g., 192.168.1.1)           | 128-bit (e.g., 2001:0db8::1)           |
| Address Format  | Decimal, dotted                      | Hexadecimal, colon-separated           |
| Address Space   | ~4.3 billion addresses               | ~340 undecillion addresses             |
| Header Size     | 20 bytes                             | 40 bytes                               |
| NAT Required    | Yes (limited addresses)              | No (massive address space)             |
| Security        | Optional                             | Built-in (IPSec mandatory)             |

---

## 📌 MAC Address
- **MAC (Media Access Control)** address is a unique identifier assigned to a network interface card (NIC).
- Format: `00:1A:2B:3C:4D:5E`
- Hardware-level address (Layer 2 - Data Link Layer)
- Assigned by device manufacturer

---

## 📌 IP Address
- An **IP address** is a unique address assigned to each device on a network to identify and locate it.
- **Types**:
  - **IPv4**: `192.168.0.1`
  - **IPv6**: `fe80::1ff:fe23:4567:890a`
- **Categories**: Public, Private, Static, Dynamic

---

## 📌 Forward Port
**Port Forwarding** allows external devices to access services on a private network through a specific port.

- Useful for:
  - Hosting servers (HTTP, FTP, game servers)
  - Remote desktop
- Example:
  - External IP:Port → Internal IP:Port  
    `203.0.113.1:8080 → 192.168.1.100:80`

---

## 📌 Nmap Command Flags
Nmap is a powerful network scanning tool.

```
-Pn -A -sV -O -oN output.txt --script <script> -vv -p <ports> -sS -sT
```

| Flag      | Description                                   |
|-----------|-----------------------------------------------|
| `-Pn`     | No ping (skip host discovery)                 |
| `-A`      | Aggressive scan (OS detection + services)     |
| `-sV`     | Version detection                             |
| `-O`      | OS detection                                  |
| `-oN`     | Output to normal file format (`output.txt`)   |
| `--script`| Run NSE (Nmap Scripting Engine) scripts       |
| `-vv`     | Very verbose output                           |
| `-p`      | Specify ports to scan (e.g., `-p 22,80,443`)  |
| `-sS`     | Stealth scan (SYN scan)                       |
| `-sT`     | TCP connect scan                              |
