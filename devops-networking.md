# 📌 DevOps Networking in Practice

## 🔹 Networking in Docker & Kubernetes
### 🐳 **Docker Networking**
Docker uses networking to enable communication between container,the host machine and external systems. It provides different network types:

| Network Type | Description |
|-------------|------------|
| **Bridge** | Default network; containers on the same bridge can communicate. |
| **Host** | Containers share the host machine’s network. |
| **Overlay** | Enables multi-host container communication (used in Swarm). |
| **Macvlan** | Assigns MAC addresses to containers, making them appear as physical devices. |
| **None** | This option provides no networking for containers that do not require network access.35 |


### ☸ **Kubernetes Networking**
This is a  mechanism that enables communication, 
scalability, security, and external access for 
containerized applications within a Kubernetes cluster

Kubernetes handles networking at scale with different models:
- **Pod-to-Pod Communication**: Uses a flat network (no NAT required).
- **Service Discovery**: Exposes services inside the cluster.
- **Ingress Controllers**: Manages external access (e.g., via Nginx Ingress).

### 📌 **Kubernetes Network Policies**
Define rules to restrict traffic flow between pods:
```yaml
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: deny-all
spec:
  podSelector: {}
  policyTypes:
    - Ingress
```

---

## 🔹 Service Discovery & Load Balancing
Service discovery ensures microservices dynamically find and connect to each other.

### 🔍 **Types of Service Discovery:**
- **Client-Side Discovery**: Services query a registry (e.g., Consul, etcd).
- **Server-Side Discovery**: Load balancers (e.g., AWS ELB, Kubernetes Services) direct traffic.

### 🎯 **Load Balancing Approaches:**
- **Round Robin** – Traffic is evenly distributed.
- **Least Connections** – Sends requests to the least busy server.
- **IP Hashing** – Uses the client’s IP to determine the target server.

Example: Kubernetes Load Balancer Service
```yaml
apiVersion: v1
kind: Service
metadata:
  name: my-service
spec:
  type: LoadBalancer
  selector:
    app: my-app
  ports:
    - protocol: TCP
      port: 80
      targetPort: 8080
```

---

## 🔹 Networking in Cloud Providers (AWS, Azure, GCP)

### 🌩 **AWS Networking**
- **VPC** – Isolated cloud network.
- **Elastic Load Balancer (ELB)** – Manages traffic distribution.
- **Route 53** – DNS and traffic routing.
- **Security Groups** – Firewall-like access controls.

### ☁ **Azure Networking**
- **Virtual Network (VNet)** – This is the fundamental building block for your private network in Azure, enabling various types of Azure resources, such as virtual machines (VMs), to securely communicate with each other, the internet, and on-premises networks

- **Azure Load Balancer** – Handles traffic between services.
- **Azure DNS** – Custom domain management.

### 🏗 **GCP Networking**
- **Google VPC** – Global, scalable network.
- **Cloud Load Balancing** – Traffic balancing across regions.
- **Cloud DNS** – Managed domain resolution.

---

## 🔹 Summary
✅ **Docker & Kubernetes** enable container networking at scale.  
✅ **Service discovery & load balancing** optimize microservice communication.  
✅ **Cloud providers** offer advanced networking tools for DevOps.  

