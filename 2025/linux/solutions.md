# 🌐 Networking for DevOps: Essentials

## 🚀 Master Networking Concepts for DevOps Engineers  

Welcome to the **Networking & DevOps Fundamentals** repository! This project is designed to help you master **essential networking concepts, protocols, and tools** that are crucial for DevOps engineers. Whether you're a beginner or looking to brush up on your skills, this repository provides **hands-on tasks, real-world examples, and practical guides** to deepen your understanding.  

---

## 📌 Topics Covered  

1. **OSI & TCP/IP Models**  
2. **Protocols and Ports for DevOps**  
3. **AWS EC2 and Security Groups**  
4. **Networking Commands Cheat Sheet**  

---

## 🔥 1. OSI & TCP/IP Models  

Understanding networking starts with grasping the **OSI (Open Systems Interconnection) model** and the **TCP/IP model**, which define how data moves across networks.

### 📜 **OSI Model: The 7 Layers & Their Functions**  
- **Application Layer** (Layer 7) → Handles network services like HTTP, FTP, and DNS.  
- **Presentation Layer** (Layer 6) → Converts data formats (e.g., encryption, compression).  
- **Session Layer** (Layer 5) → Manages sessions and connections.  
- **Transport Layer** (Layer 4) → Ensures reliable data transfer (TCP, UDP).  
- **Network Layer** (Layer 3) → Routes packets (IP addresses, routers).  
- **Data Link Layer** (Layer 2) → Manages MAC addresses and Ethernet.  
- **Physical Layer** (Layer 1) → Deals with physical network components (cables, hubs).  

### 🌍 **TCP/IP Model & Mapping to OSI Model**  
- **Application Layer** → Merges OSI’s Application, Presentation, and Session layers.  
- **Transport Layer** → TCP/UDP ensures data reliability.  
- **Internet Layer** → Handles routing via IP.  
- **Network Access Layer** → Manages MAC addressing, Ethernet, and physical connectivity.  

### 🔍 **Real-World Examples**  
| Layer | Example |
|-------|---------|
| **Application** | HTTP/HTTPS for web browsing |
| **Transport** | TCP for reliable transfer, UDP for streaming |
| **Network** | IP for routing packets |
| **Data Link** | Ethernet for local network communication |
| **Physical** | Cables, switches, hubs |

---

## 🚀 2. Protocols and Ports for DevOps  

A solid understanding of **networking protocols and ports** is essential for DevOps engineers.

### 🔗 **Common Protocols & Their Ports**  
| Protocol | Port | Purpose |
|----------|------|---------|
| **HTTP** | 80 | Web communication |
| **HTTPS** | 443 | Secure web communication |
| **FTP** | 21 | File transfer |
| **SSH** | 22 | Secure remote access |
| **DNS** | 53 | Domain name resolution |

### 🎯 **Relevance to DevOps**  
- **HTTP/HTTPS** → Used in web applications, REST APIs, and microservices.  
- **SSH** → Essential for remote server management, automation, and CI/CD pipelines.  
- **DNS** → Helps with service discovery, load balancing, and scaling applications.  

---

## 🏗️ 3. AWS EC2 and Security Groups  

### 🖥️ **Step-by-Step Guide: Launching an EC2 Instance**  
1. **Log in to AWS Management Console**  
2. Navigate to **EC2** and click **"Launch Instance"**  
3. **Choose an Amazon Machine Image (AMI)** and instance type  
4. **Configure instance details and add storage**  
5. **Configure Security Groups** to allow SSH (Port 22) and HTTP (Port 80)  
6. **Launch the instance** and connect using SSH  

### 🔐 **Configuring Security Groups**  
Security groups in AWS act as **virtual firewalls** that control inbound and outbound traffic.

✅ **Best Practices:**  
- Define **specific inbound rules** to allow necessary services (e.g., SSH, HTTP).  
- **Restrict access** to specific IP addresses to enhance security.  

📌 **Example Security Group Rules:**  
| Protocol | Port | Source |
|----------|------|--------|
| **SSH** | 22 | Your IP (e.g., `192.168.1.1/32`) |
| **HTTP** | 80 | Anywhere (`0.0.0.0/0`) |
| **HTTPS** | 443 | Anywhere (`0.0.0.0/0`) |

---

## 📖 4. Networking Commands Cheat Sheet  

Networking commands are essential for troubleshooting, monitoring, and managing network configurations.  

### 🔍 **Essential Commands & Usage**  

#### 🖥️ **1. Check Connectivity (Ping)**
```sh
ping google.com
```
✅ Tests if a host is reachable over the network.  

#### 🌍 **2. Trace Packet Route (Traceroute)**
```sh
traceroute google.com   # Linux/macOS
tracert google.com      # Windows
```
✅ Shows the path packets take to reach a destination.  

#### 📡 **3. View Network Connections (Netstat)**
```sh
netstat -tuln
```
✅ Displays active connections, listening ports, and routing tables.  

#### 🔗 **4. Perform HTTP Requests (Curl)**
```sh
curl -I https://google.com
```
✅ Fetches HTTP headers for troubleshooting web services.  

#### 🌐 **5. Perform DNS Lookup (Dig & Nslookup)**
```sh
dig google.com
nslookup google.com
```
✅ Resolves domain names to IP addresses.  
