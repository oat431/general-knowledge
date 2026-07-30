---
tags:
  - computer-science
  - advance
  - computer-systems
  - networks
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว333"]
---

# Computer Systems and Networks — ระบบคอมพิวเตอร์และเครือข่าย

> *"The network is the computer."* — John Gage, Sun Microsystems (1984)

A computer system (ระบบคอมพิวเตอร์) is more than the machine on your desk — it is the integration of **hardware** (ฮาร์ดแวร์), **software** (ซอฟต์แวร์), and the people who use them. A computer network (เครือข่ายคอมพิวเตอร์) connects these systems so they can share data and resources, from a home Wi-Fi network to the global Internet.

This note covers the major hardware components, software categories, operating systems, network types (LAN/WAN), the TCP/IP protocol suite, IP addressing, DNS, HTTP/HTTPS, the client-server model, and foundational cybersecurity concepts (ความมั่นคงปลอดภัยไซเบอร์).

---

## 1 | Course Coverage

### ม.6 (ว333)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Hardware, software, operating systems, network fundamentals | Identify components, explain LAN/WAN, read IP addresses |
| **Semester 2** | TCP/IP, DNS, HTTP/HTTPS, client-server, cybersecurity | Trace a web request, identify threats, explain encryption |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ฮาร์ดแวร์ | Hardware | Physical components |
| ซอฟต์แวร์ | Software | Programs / instructions |
| หน่วยประมวลผลกลาง | CPU (Central Processing Unit) | The "brain" |
| หน่วยความจำ | RAM (Random Access Memory) | Volatile working memory |
| ระบบปฏิบัติการ | Operating System (OS) | Windows, macOS, Linux, Android |
| เครือข่าย | Network | Connected computers |
| เครือข่ายบริเวณเครื่อง | LAN (Local Area Network) | Small/local |
| เครือข่ายบริเวณกว้าง | WAN (Wide Area Network) | Large/geographic |
| พิธีการ | Protocol | Communication rules |
| โดเมน | Domain | e.g. `example.com` |
| การเข้ารหัส | Encryption | Scramble for secrecy |
| ไฟร์วอลล์ | Firewall | Filters network traffic |

---

## 3 | Key Concepts

### 3.1 Hardware Components (ฮาร์ดแวร์)

| Component | Thai | Role |
|---|---|---|
| **CPU** | หน่วยประมวลผลกลาง | Executes instructions (ALU + control unit) |
| **RAM** | หน่วยความจำหลัก | Temporary working storage; volatile |
| **Storage** | หน่วยเก็บข้อมูล | SSD/HDD — persistent storage |
| **Input devices** | อุปกรณ์นำเข้า | Keyboard, mouse, microphone |
| **Output devices** | อุปกรณ์แสดงผล | Monitor, speaker, printer |
| **Motherboard** | เมนบอร์ด | Connects all components |
| **GPU** | หน่วยประมวลผลกราฟิก | Graphics & parallel computation |

A common mental model: the **CPU** is the brain, **RAM** is the short-term desk, **storage** is the filing cabinet, and the **bus** (บัส) is the nervous system connecting them.

### 3.2 Software Types (ซอฟต์แวร์)

- **System software** (ซอฟต์แวร์ระบบ) — manages hardware: operating systems, device drivers, utilities.
- **Application software** (ซอฟต์แวร์ประยุกต์) — performs user tasks: browsers, word processors, games.
- **Firmware** (เฟิร์มแวร์) — low-level code embedded in hardware (BIOS, router OS).

### 3.3 Operating Systems (ระบบปฏิบัติการ)

The operating system (OS, ระบบปฏิบัติการ) manages hardware resources and provides services to applications: process scheduling, memory management, file systems, and a user interface.

| OS | Examples | Target |
|---|---|---|
| Desktop | Windows, macOS, Linux (Ubuntu) | PCs & laptops |
| Mobile | Android, iOS | Phones & tablets |
| Embedded | RTOS, router firmware | Specialized devices |

### 3.4 Network Types (ประเภทเครือข่าย)

| Type | Thai | Scope | Example |
|---|---|---|---|
| **LAN** | เครือข่ายบริเวณเครื่อง | Single building/campus | School Wi-Fi |
| **WAN** | เครือข่ายบริเวณกว้าง | City/country/global | The Internet |
| **PAN** | เครือข่ายส่วนบุคคล | A few meters | Bluetooth headphones |
| **WLAN** | เครือข่ายไร้สาย | Wireless LAN | Wi-Fi hotspot |

### 3.5 The TCP/IP Protocol Suite

The Internet uses the **TCP/IP** model — a stack of four layers, each with a responsibility:

| Layer | Role | Protocols / Devices |
|---|---|---|
| **Application** | User-facing services | HTTP, HTTPS, DNS, SMTP |
| **Transport** | Reliable/unordered delivery | TCP (reliable), UDP (fast) |
| **Internet** | Routing across networks | IP, routers |
| **Network access** | Physical transmission | Ethernet, Wi-Fi, switches |

When you load a webpage, your data travels **down** the sender's stack, across the network, and **up** the receiver's stack — each layer adding/stripping its own header (encapsulation).

### 3.6 IP Addressing (การกำหนดที่อยู่ IP)

An **IP address** (ที่อยู่ IP) uniquely identifies a device on a network.

- **IPv4:** 32-bit, written as four octets, e.g. `192.168.1.10` — about 4.3 billion addresses.
- **IPv6:** 128-bit, e.g. `2001:db8::1` — virtually unlimited.
- **Private vs public:** `192.168.x.x`, `10.x.x.x`, `172.16-31.x.x` are private (internal); the rest are public (Internet-routable).
- **DNS (Domain Name System):** translates human names to IPs — `google.com` → `142.250.x.x`.

### 3.7 HTTP/HTTPS and the Client-Server Model

The **client-server model** (โมเดลไคลเอนต์-เซิร์ฟเวอร์): a **client** (your browser) requests a resource; a **server** (a remote computer) responds.

- **HTTP** (HyperText Transfer Protocol) — the rules for requesting and serving web pages.
- **HTTPS** — HTTP over **TLS/SSL** (การเข้ารหัส) — the connection is encrypted, shown by 🔒 in the browser.

A simplified request/response:

```
1. Browser → DNS: "What is the IP of example.com?"
2. DNS → Browser: "93.184.216.34"
3. Browser → Server (TCP connection on port 443):
   GET / HTTP/1.1
   Host: example.com
4. Server → Browser: HTML page (200 OK)
5. Browser renders the page
```

### 3.8 Cybersecurity Basics (ความมั่นคงปลอดภัยไซเบอร์)

| Threat | Thai | Description |
|---|---|---|
| **Malware** | มัลแวร์ | Viruses, worms, trojans, ransomware |
| **Phishing** | ฟิชชิง | Fraudulent messages tricking users |
| **DDoS** | การโจมตีแบบ DDoS | Overwhelm a server with traffic |
| **MITM** | มิดเดิลแมน | Intercept communication |
| **SQL injection** | เอสคิวแอลอินเจกชัน | Malicious DB queries |

**Defenses:**

- **Encryption** (การเข้ารหัส) — convert plaintext to ciphertext using a key (AES, RSA).
- **Firewall** (ไฟร์วอลล์) — filter incoming/outgoing traffic by rules.
- **Authentication** (การยืนยันตัวตน) — passwords, 2FA/MFA, biometrics.
- **Updates/Patches** — fix known vulnerabilities.
- **Backup** (สำรองข้อมูล) — recover from ransomware or failure.

The **CIA triad** (สามเสาหลัก) of security: **Confidentiality** (ปกปิด), **Integrity** (ความถูกต้อง), **Availability** (พร้อมใช้งาน).

---

## 4 | Common Problem Types

### Type 1: Decode an IP Address

> Given `192.168.0.5`, identify the IP version, class, and whether it is private.

**Solution:**
```python
ip = "192.168.0.5"
parts = ip.split(".")
is_ipv4 = len(parts) == 4 and all(p.isdigit() and 0 <= int(p) <= 255 for p in parts)
private = ip.startswith(("10.", "172.16.", "172.17.", "172.31.", "192.168."))
print(f"IPv4: {is_ipv4}, Private: {private}")
# IPv4: True, Private: True
```

### Type 2: Trace a Web Request (Client-Server)

> List the ordered steps when a user types `https://school.ac.th` and presses Enter.

**Solution (pseudocode flow):**
```
1. Browser checks DNS for school.ac.th → IP (e.g., 203.154.x.x)
2. TCP three-way handshake to server:443
3. TLS handshake establishes encrypted session
4. Browser sends: GET / HTTP/1.1  + Host header
5. Server responds: HTTP/1.1 200 OK + HTML body
6. Browser parses HTML, fetches CSS/JS/images (repeat 4-5)
7. Page rendered to user
```

### Type 3: Simple Port Scanner (Educational)

> Scan a small list of common ports to see which are open (for learning only — never scan hosts you don't own).

**Solution:**
```python
import socket

def scan(host, ports):
    for p in ports:
        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
        s.settimeout(1)
        result = s.connect_ex((host, p))
        status = "OPEN" if result == 0 else "closed"
        print(f"Port {p}: {status}")
        s.close()

# scan("127.0.0.1", [80, 443, 22, 3306])  # localhost only
```

---

## 5 | Cross-Links

- [[10_Databases]] — databases run as server software over networks
- [[11_Artificial_Intelligence]] — AI services delivered over client-server APIs
- [[12_Digital_Citizenship]] — cybersecurity threats and safe online behavior
- [[../../Fundamental/03_Number_Systems|Mathematics: Number Systems]] — binary/hex for IP and addressing
