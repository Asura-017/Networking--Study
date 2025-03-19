# 📌 Network Protocols & Communication

## 🔹 TCP/IP Model vs. OSI Model
Networking models define how devices communicate. The two main models are:

### 1️⃣ **TCP/IP Model** (4 Layers)
The TCP/IP model is the foundation of the internet and modern networking.

| Layer | Description |
|-------|------------|
| **Application** | Handles data exchange between applications (HTTP, FTP, SMTP) |
| **Transport** | Ensures reliable data transfer (TCP, UDP) |
| **Internet** | Manages IP addressing  and the routing of data packets across the network (IP, ICMP) |
| **Network Access** | Deals with physical transmission (Ethernet, Wi-Fi) |

### 2️⃣ **OSI Model** (7 Layers)
The OSI model provides a more detailed breakdown:

| Layer | Function |
|--------|-----------|
| **7. Application** | Provides User interaction with network services (HTTP, DNS) |
| **6. Presentation** | Converts data to and from the Application layer, handling encryption, compression, and formatting. (SSL, TLS) |
| **5. Session** | Establishes, manages, and terminates connections/Sessions between applications and  devices |
| **4. Transport** | Ensures reliable data transmission between devices. (TCP, UDP) |
| **3. Network** | Logical addressing and routing (IP, ICMP) |
| **2. Data Link** | MAC addressing and switching (Ethernet, ARP) |
| **1. Physical** | Hardware transmission (Cables, Wi-Fi) |

---

## 🔹 Common Network Protocols

### 1️⃣ **HTTP & HTTPS** (Hypertext Transfer Protocol)
- **HTTP** (Port 80) – Used for web communication.
- **HTTPS** (Port 443) – Secure HTTP using SSL/TLS encryption.

### 2️⃣ **FTP (File Transfer Protocol)**
- **FTP** (Port 21) – Transfers files between computers.
- **SFTP (Secure FTP)** – Uses SSH for secure file transfers.

### 3️⃣ **SSH (Secure Shell)**
- **SSH** (Port 22) – Secure remote access to servers.
- Used for managing cloud and DevOps environments.

### 4️⃣ **SMTP (Simple Mail Transfer Protocol)**
- **SMTP** (Port 25, 465, 587) – Sends emails.
- Works with IMAP/POP3 for email retrieval.

### 5️⃣ **SNMP (Simple Network Management Protocol)**
- **SNMP** (Port 161) – Monitors network devices (routers, switches).
- Used in network administration.

---

## 🔹 VPNs & Firewalls: Importance in Security

### 🛡 **VPN (Virtual Private Network)**
- Encrypts internet traffic for **secure remote access**.
- Used in **corporate networks** and **secure cloud connections**.
- Common protocols: **OpenVPN, IPsec, WireGuard**.

### 🔥 **Firewalls**
- **Network Security Devices** that filter traffic.
- Types:
  - **Packet Filtering** – Inspects data packets.
  - **Stateful Inspection** – Tracks connection state.
  - **Next-Gen Firewalls (NGFW)** – Advanced filtering with IDS/IPS.

---

## 🔹 Summary
✅ **TCP/IP and OSI models** define how networks communicate.
✅ **Common protocols** like HTTP, SSH, and SMTP enable internet services.
✅ **VPNs and firewalls** enhance network security in cloud and DevOps environments.

