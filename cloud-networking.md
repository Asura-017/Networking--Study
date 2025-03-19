# 📌 Cloud Networking Concepts

## 🔹 Virtual Private Cloud (VPC)
A **Virtual Private Cloud (VPC)** is a logically isolated section within a public cloud provider where you can deploy resources securely.

### 🌐 **Key Features:**
- **Subnetting:** Divides VPC into smaller networks for better control.
- **Route Tables:** Direct traffic between subnets and external networks.
- **Network ACLs & Security Groups:** Control inbound/outbound traffic.
- **Internet Gateway (IGW):** Enables external internet access.

### 🔧 **Common Cloud Providers:**
- **AWS VPC** – Amazon Web Services
- **Azure VNet** – Microsoft Azure
- **Google VPC** – Google Cloud Platform

---

## 🔹 Load Balancers
Load balancers distribute incoming traffic across multiple servers to ensure high availability and reliability and reduces the lod which a server carries.

### 📌 **Types of Load Balancers:**
1️⃣ **Application Load Balancer (ALB)** – Operates at Layer 7 (HTTP/HTTPS).  
2️⃣ **Network Load Balancer (NLB)** – Works at Layer 4 (TCP/UDP).  
3️⃣ **Classic Load Balancer (CLB)** – Older AWS version, used for legacy applications.

### 🚀 **Benefits:**
- Improves performance by distributing traffic efficiently.
- Ensures fault tolerance by rerouting traffic during server failures.
- Enhances security by blocking malicious traffic before it reaches the backend.

---

## 🔹 Content Delivery Networks (CDN)
A **Content Delivery Network (CDN)** is a distributed network of servers that improves web performance by caching content across distributed global servers.

### 🌎 **How CDNs Work:**
1️⃣ User requests a webpage.  
2️⃣ CDN delivers cached content from the nearest edge location.  
3️⃣ Reduces latency and improves load times.

### 🛠 **Popular CDN Providers:**
- **Cloudflare CDN** – Security and DDoS protection.
- **AWS CloudFront** – Integrated with AWS services.
- **Akamai CDN** – Used by large enterprises.

---

## 🔹 DNS Management in Cloud Platforms
DNS (Domain Name System) is responsible for translating human-readable domain names (e.g., example.com) into IP addresses (192.168.1.1) that computers use to communicate. Cloud-based DNS services provide high availability, scalability, and performance for managing domain names.



### 🔹 **Cloud-based DNS Services:**
- **Amazon Route 53** – Scalable and highly available DNS.
- **Azure DNS** – Fast, secure name resolution for Azure resources.
- **Google Cloud DNS** – Low-latency, high-availability DNS.

### 🏗 **DNS Features:**
- **A Record:** Maps domain names to IPv4 addresses.
- **CNAME Record:** Aliases one domain to another.
- **MX Record:** Directs email traffic.
- **TTL (Time To Live):** Controls DNS caching duration.

---

## 🔹 Summary
✅ **VPCs provide secure cloud networking environments.**  
✅ **Load balancers improve scalability and performance.**  
✅ **CDNs reduce latency and enhance website speed.**  
✅ **Cloud DNS services optimize domain resolution.**  

