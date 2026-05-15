# 🚀 Day 15 – Advanced VPC Networking (NAT Gateway & Route Tables)

---

# 📌 Overview

On Day 15, I explored advanced AWS VPC networking concepts including:

* NAT Gateway
* Route Tables
* Public & Private Subnets
* Internet Gateway
* Secure cloud network architecture

This day focused on designing secure and scalable enterprise-level cloud networks.

---

# ☁️ What is VPC Networking?

Amazon VPC (Virtual Private Cloud) allows users to create isolated cloud networks inside AWS.

It helps:

* Secure resources
* Control traffic
* Build scalable architectures
* Isolate public/private services

---

# 🌐 Core Networking Components

## 1. VPC

Logical isolated network inside AWS.

---

## 2. Public Subnet

Subnet connected to internet using Internet Gateway.

### Examples:

* Web servers
* Load balancers

---

## 3. Private Subnet

Subnet without direct internet access.

### Examples:

* Databases
* Backend services

---

## 4. Internet Gateway (IGW)

Allows internet connectivity for public subnet resources.

---

## 5. NAT Gateway

Allows private subnet instances to access internet securely without exposing them publicly.

---

## 6. Route Tables

Controls network traffic routing between subnets and internet.

---

# ⚙️ VPC Networking Workflow

```plaintext id="c1b4v8"
Internet
    ↓
Internet Gateway
    ↓
Public Subnet
    ↓
NAT Gateway
    ↓
Private Subnet
```

---

# 🌐 Real-World Project – Secure Multi-Tier Architecture

---

# 🏗️ Project Objective

Build a secure enterprise cloud architecture where:

* Public subnet hosts web servers
* Private subnet hosts databases
* NAT Gateway provides secure outbound internet
* Route tables control traffic
* Security groups restrict access

---

# 🧠 Project Architecture

```plaintext id="6rfyhl"
Users
   ↓
Load Balancer
   ↓
Public EC2 Servers
   ↓
NAT Gateway
   ↓
Private Database Servers
```

---

# 🔐 Security Features Implemented

* Private subnet isolation
* NAT Gateway outbound-only access
* Route table restrictions
* Security Groups
* Network ACLs

---

# 📊 Monitoring & Management

## CloudWatch Monitoring

Tracks:

* Network traffic
* Packet flow
* NAT usage
* EC2 health

---

# 🔟 Real-World Use Cases

1. Enterprise applications
2. Banking infrastructure
3. Secure backend systems
4. Multi-tier architectures
5. SaaS applications
6. AI/ML secure networking
7. DevOps environments
8. Kubernetes clusters
9. E-commerce platforms
10. Hybrid cloud networking

---

# 💻 Example Route Table

| Destination    | Target           |
| -------------- | ---------------- |
| 0.0.0.0/0      | Internet Gateway |
| Private Subnet | NAT Gateway      |

---

# 🧪 Hands-On Tasks

## Task 1

Create VPC.

---

## Task 2

Create Public & Private Subnets.

---

## Task 3

Attach Internet Gateway.

---

## Task 4

Create NAT Gateway.

---

## Task 5

Configure Route Tables.

---

## Task 6

Launch EC2 instances.

---

# 🧠 What I Learned

* Advanced VPC architecture
* NAT Gateway working
* Route table configuration
* Secure subnet isolation
* Enterprise cloud networking

---

# 🚀 Next Step (Day 16)

* AWS Auto Scaling & Load Balancing

---

# 📌 Author

**Sankar S**
Cloud & AI Learning Journey 🚀
