# Study List
---
## **Github**

### **Version control**
### **Git Branching**
### **Git Commands**

---

## **Automation**

### **Continuous Integration / Continuous Deployment**
### **CI/CD Pipeline & Github**
### **Endocode Project**
### **Automated Testing / Deployment: Jenkins**
### **Gitlab**

---
## **Infrastruction as Code**

### **Terraform**
### **CloudFormation**

---
## **Linux**

### **Linus Operating Systems**
### **Linux Commands**

---
## **Python**

### **Flask**
### **Django**

---
## **Distributed Data Storage**

### **Hadoop**
### **Ceph**

---
## **NoSQL**

### **SQL v NoSQL**
### **MongoDB**
### **Redis**
### **Cassandra**

---
## **Data Aggregation**

### **ElasticSearch**
### **Kafka**

---
## **Scaling & Running traditional RDMS**

### **PostgreSQL**
### **MySQL**

---
## **Containerisation: Docker**

### **Virtual Machines / Instances**
### **Docker Containers & Docker Images**
### **Dockerhub**
### **Dockerfiles**
### **Docker Compose**
### **Docker Commands**

---
## **Container Orchestration: Kubernetes**

### **K8s Cluster Structure:**
Nodes / Containers / Docker / VM
### **Helm**
### **Kubectl**
### **Openshift, GKE**

---
## **Monitoring & Logging & Alerting**

### **Incident Management Toolsets**
### **Prometheus**
### **Grafana**
### **Kibana**
### **DataDog**
### **Argo**
### **Istio**

---
## **Software Distribution**

### Package Management
### Distribution at Scale

---
## **Configuration Management**

### **Push or Pull Configuration**

There are 2 ways to set up an environment for server farms:
1. **Pull configuration:** A Master server containing instructions, where each server contains client software for communicating with the Master server for updating the config of slave servers
2. **Push configuration:** A Master server contains instructions, but no client software is needed on client servers. The Master server simply pushes out instructions to the slave servers to force restructuring

### **Ansible is a Push Configuration tool**
Ansible is an Operations tool for DevOps.
It uses code scripting to describe the installation and setup of multiple servers in multiple locations.
It is essentially 1 script for executing a consistent environment.

### **Chef & Puppet are Pull configuration tools**
Pull Configurations use a Master/Slave Architecture where the Master server connection to the client server in a remote slave enironment. 
The Client server pulls updates from the Master server

The Advantages of a Push configuration is that there's no overhead weight of a client installed on the remote servers, which in case would have to constantly communicate back with the MAster environment.

### **Ansible Architecture**
- A **Local Machine** contains all of the instructions for pushing out to the remote servers (Module & Inventory).
- **Nodes** are the remote systems to be configured, they are controlled by the local machine.
- **Modules** are the configuration code files called consistent PlayBooks.
- **Inventory** is a document that groups the nodes under specific labels.
- The Local Machine connect to nodes through an **SSH client**.

### **Ansible Playbook**
- A Playbook is a set of instructions which configure the nodes.
- Written in YAML.

**Play 1 & Play 2**
In each Play we:
- Define nodes to target eg. [webserver] [databaseserver] (NAMES)
- Within each server environment we define a task for each we wish to execute (eg. install apache task, start apache task, install MySQL task)
- Then execute each set of instructions (Yum:)

### **Inventory**
### **How Ansible works**
### **Ansible v Chef or Puppet**

---
## **Networking**

### **Domain Name System**
### **Routing / Privacy / Security**
### **Transport Layer Security (TSL) [Formally SSL]**
### **Secure Shell Protocol (SSH)**
