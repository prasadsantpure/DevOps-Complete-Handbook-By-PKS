# DevOps-Complete-Handbook-By-PKS
 This repository contains a complete DevOps learning handbook covering everything from foundational Linux skills to advanced Kubernetes, Terraform, CI/CD pipelines, DevSecOps, cloud architecture, and real production-grade projects.  Designed for students, self-learners, and professionals who want to master DevOps end-to-end.

# 1. Introduction to DevOps

## 1.1 What is DevOps?
DevOps is a cultural, organizational, and technical methodology that integrates **Development (Dev)** and **Operations (Ops)** teams to deliver software faster, more reliably, and with higher quality.

DevOps focuses on:
- Collaboration and shared ownership  
- Automation of the software delivery lifecycle  
- Continuous Integration and Continuous Delivery (CI/CD)  
- Monitoring, observability, and quick feedback loops  
- Infrastructure as Code (IaC)  
- Cloud-native architectures  

DevOps is not:
- A tool  
- A team name  
- A person  
- A single practice  

It is a **culture + toolset + process** that transforms how companies build and run software.

---

## 1.2 Why DevOps?
Traditional software development often involves:
- Long release cycles  
- Slow feedback loops  
- Siloed teams  
- Difficult deployments  
- Unreliable releases  

DevOps solves these with:
- Automation  
- Continuous integration  
- Standardized workflows  
- Infrastructure automation  
- Cloud platforms  
- Containerization  

---

## 1.3 DevOps Lifecycle
The DevOps lifecycle includes:

1. **Plan** – Requirements, roadmaps, issue tracking  
2. **Code** – Version control, code reviews  
3. **Build** – Build automation, package creation  
4. **Test** – Automated tests  
5. **Release** – Artifact management  
6. **Deploy** – CI/CD pipelines  
7. **Operate** – Infrastructure management, cloud provisioning  
8. **Monitor** – Observability, alerting  
9. **Feedback** – Continuous improvements  

---

## 1.4 DevOps vs Traditional IT
| Traditional | DevOps |
|-------------|---------|
| Siloed teams | Unified teams |
| Manual deployments | Automated CI/CD |
| Slow feedback | Fast feedback |
| Manual infra | IaC |
| Rare releases | Frequent releases |

---

## 1.5 DevOps Pillars
- Culture (collaboration)  
- Automation  
- Measurement  
- Sharing  
- Cloud  
- Containers  
- Infrastructure as Code  
- Continuous improvement  

---

## 1.6 DevOps Tool Categories
DevOps tools can be grouped into:

- **Version Control**: Git, GitHub, GitLab  
- **CI/CD**: Jenkins, GitHub Actions, GitLab CI  
- **Containers**: Docker  
- **Orchestration**: Kubernetes  
- **Cloud**: AWS, Azure, GCP  
- **Infrastructure as Code**: Terraform, CloudFormation  
- **Config Management**: Ansible, Chef, Puppet  
- **Monitoring**: Prometheus, Grafana, CloudWatch  
- **Logging**: ELK, EFK  
- **Security**: Trivy, Checkov, Vault  

---

## 1.7 DevOps Benefits
- Faster time to market  
- Higher deployment frequency  
- Lower failure rate  
- Faster recovery times  
- Improved culture  
- Scalability and cost optimization  


# 2. SDLC, Agile, DevOps Culture

## 2.1 Software Development Life Cycle (SDLC)
The SDLC defines the stages involved in building software from idea to deployment and maintenance.

### SDLC Phases:
1. **Requirement Gathering**  
2. **Design**  
3. **Development**  
4. **Testing**  
5. **Deployment**  
6. **Maintenance**

DevOps enhances SDLC by enabling:
- Continuous feedback  
- Automated testing  
- Continuous integration & delivery  
- Faster iterations  

---

## 2.2 Agile Methodology
Agile is an iterative software development methodology focused on:
- Incremental releases  
- Customer collaboration  
- Responding to change  

### Popular Agile frameworks:
- **Scrum** (sprints, standups, product owner, scrum master)
- **Kanban** (continuous flow, WIP limits)
- **XP (Extreme Programming)**

---

## 2.3 Agile vs DevOps
| Agile | DevOps |
|-------|--------|
| Focus on development process | Focus on end-to-end delivery |
| Sprints & iteration | Automation & collaboration |
| Frequent code delivery | Continuous deployment & monitoring |
| Developers + product team | Developers + operations |

Agile improves **software creation**, while DevOps improves **software delivery**.

---

## 2.4 DevOps Culture
DevOps is fundamentally about **culture change**, not tools.

### Principles:
- Collaboration between Dev, Ops, QA, and Security  
- Shared responsibility  
- Continuous learning  
- Blameless postmortems  
- Automation mindset  

---

## 2.5 CALMS Framework
A model that describes DevOps culture:

| Component | Meaning |
|-----------|----------|
| **C** | Culture |
| **A** | Automation |
| **L** | Lean practices |
| **M** | Measurement |
| **S** | Sharing |

---

## 2.6 DevOps & CI/CD Relationship
DevOps enables continuous integration and continuous delivery pipelines:

- CI automates testing and integration  
- CD automates deployments and releases  
- Infrastructure automation enables fast rollouts  
- Monitoring provides feedback loops  

---

## 2.7 DevOps Goals
- Deliver software faster  
- Reduce risk  
- Improve reliability  
- Increase automation  
- Lower costs  
- Minimize downtime  

---

## 2.8 DevOps Anti-Patterns (What NOT to do)
- Treating DevOps as a separate team  
- Over-reliance on manual processes  
- Not investing in monitoring  
- No documentation or knowledge-sharing  
- Only focusing on tools instead of culture  

---

## 2.9 Key DevOps Metrics (DORA Metrics)
DORA metrics measure DevOps performance:

| Metric | Description |
|--------|-------------|
| Deployment frequency | How often you deploy |
| Lead time for changes | Time from commit → production |
| Change failure rate | % deployments that fail |
| MTTR | Mean Time To Recovery |

Top companies measure and optimize these continuously.

---



# 3. Core DevOps Tools

DevOps relies on a rich set of tools across the entire software delivery lifecycle.  
This chapter provides a complete overview of the essential tools every DevOps engineer must know.

---

## 3.1 Version Control Systems (VCS)

### **Git**
Git is the most widely used distributed version control system.

Key commands:
- `git clone`
- `git add`
- `git commit`
- `git push`
- `git pull`
- `git branch`
- `git merge`
- `git rebase`

### **Git Hosting Platforms**
- **GitHub**
- **GitLab**
- **Bitbucket**

Features:
- Pull Requests
- Code reviews
- Branch protection
- Webhooks

---

## 3.2 CI/CD Tools

### **Jenkins**
- Most widely used CI/CD automation tool  
- Supports pipelines (Groovy)  
- Highly extensible with plugins  

### **GitHub Actions**
- GitHub-native CI/CD  
- Uses YAML workflows  
- Easy cloud deployments  

### **GitLab CI**
- Fully integrated CI/CD  
- Runner-based architecture  

### **CircleCI, TravisCI, Azure DevOps**
Other major platforms depending on project needs.

---

## 3.3 Containerization Tools

### **Docker**
- Build, ship, and run containers  
- Dockerfile for image definition  
- Docker Hub/ECR/GCR registries  

### **Container Runtime Options**
- Docker Engine  
- containerd  
- CRI-O  

---

## 3.4 Container Orchestration Tools

### **Kubernetes**
The most powerful orchestration system:
- Auto-scaling  
- Rolling deployments  
- Self-healing  
- Service discovery  
- Persistent storage  

### Others (less common):
- Docker Swarm  
- Nomad  
- OpenShift  

---

## 3.5 Infrastructure as Code (IaC)

### **Terraform**
- Cloud-agnostic IaC  
- Manages AWS, Azure, GCP, Kubernetes  
- Uses declarative language (HCL)  
- State management  

### **AWS CloudFormation**
- AWS-native IaC  

### **Pulumi**
- IaC using programming languages  

---

## 3.6 Configuration Management Tools

### **Ansible**
- Agentless  
- YAML playbooks  
- Easy to learn  
- Great for provisioning & automation  

### **Chef, Puppet, SaltStack**
More complex, agent-based options.

---

## 3.7 Secrets Management

- HashiCorp Vault  
- AWS Secrets Manager  
- AWS SSM Parameter Store  
- Kubernetes Secrets  

Best practices:
- Never hardcode secrets  
- Rotate keys regularly  
- Use encryption at rest and transit  

---

## 3.8 Monitoring & Logging Tools

### **Monitoring**
- Prometheus  
- Grafana  
- CloudWatch  
- Datadog  
- New Relic  

### **Logging**
- ELK stack (Elasticsearch, Logstash, Kibana)  
- EFK stack (Elasticsearch, Fluentd, Kibana)  
- Loki + Grafana  

---

## 3.9 Container Registries

- Docker Hub  
- AWS ECR  
- GitHub Packages  
- Google Container Registry (GCR)  
- Azure Container Registry (ACR)

---

## 3.10 Collaboration Tools

- Jira (issue tracking)  
- Confluence (documentation)  
- Slack (communication)  
- Teams (communication)  

---

## 3.11 Artifact Repositories

- Nexus  
- JFrog Artifactory  

Used to store:
- Build artifacts  
- JAR/WAR files  
- Helm charts  

---

## 3.12 Summary

A DevOps engineer must master:
- Git  
- CI/CD (Jenkins/GitHub Actions)  
- Docker  
- Kubernetes  
- Terraform  
- AWS  
- Monitoring & logging  

These form the backbone of modern DevOps workflows.

---



# 4. Linux Essentials

Linux is the backbone of DevOps, cloud, and containerized environments.  
A DevOps engineer must be deeply comfortable with Linux systems, commands, services, permissions, and troubleshooting.

---

## 4.1 Linux File System Hierarchy

Common directories:
- `/` – Root directory  
- `/home` – User home directories  
- `/etc` – Configuration files  
- `/var` – Logs, variable data  
- `/usr` – User binaries, libraries  
- `/bin`, `/sbin` – System binaries  
- `/opt` – Optional packages  
- `/mnt`, `/media` – Mounted storage  

---

## 4.2 Basic Linux Commands

### File & Directory
- `ls`, `cd`, `pwd`
- `cp`, `mv`, `rm`
- `mkdir`, `rmdir`
- `touch`
- `cat`, `less`, `head`, `tail`

### Permissions
- `chmod`
- `chown`
- `umask`

Modes:
- r (read)
- w (write)
- x (execute)

---

## 4.3 File Permissions

### Numeric (octal):
- `7` = rwx  
- `6` = rw-  
- `5` = r-x  
- `4` = r--  

Example:
```
chmod 755 script.sh
```

---

## 4.4 Users & Groups

- Add user: `useradd`, `adduser`
- Add group: `groupadd`
- Switch user: `su`, `sudo`
- Modify user: `usermod`
- Delete user: `userdel`

---

## 4.5 Processes & Services

### Process Management
- `ps`, `top`, `htop`
- `kill`, `killall`
- `nice`, `renice`

### System Services (systemd)
- `systemctl start`
- `systemctl stop`
- `systemctl enable`
- `systemctl status`

---

## 4.6 Linux Networking

Commands:
- `ip a`
- `ip r`
- `ss -tuln`
- `ping`
- `netstat` (older)
- `curl`, `wget`
- `dig`, `nslookup`

---

## 4.7 Package Management

### Debian-based:
- `apt update`, `apt install`

### RedHat-based:
- `yum install`
- `dnf install`

---

## 4.8 Disk, Storage & File Systems

### Disk Commands
- `df -h` (disk usage)
- `du -sh` (directory size)
- `lsblk` (block devices)
- `mount`, `umount`
- `fdisk`, `parted`

### File System Creation
```
mkfs.ext4 /dev/sdb1
```

---

## 4.9 Log Management

Logs stored under `/var/log`:
- `syslog`
- `auth.log`
- `kern.log`
- `messages`

### Commands:
- `tail -f`
- `grep`
- `journalctl`

---

## 4.10 Shell Scripting (Bash)

Basic structure:
```bash
#!/bin/bash
echo "Hello"
```

### Topics:
- Variables  
- Arrays  
- Loops  
- If/else  
- Functions  
- Cron jobs  

---

## 4.11 Cron Jobs

Scheduling tasks:
```
crontab -e
```

Format:
```
* * * * * command
```

Example:
```
0 2 * * * /opt/backup.sh
```

---

## 4.12 SSH & Remote Access

- Key generation: `ssh-keygen`
- Copy key: `ssh-copy-id`
- Connect: `ssh user@host`

### Harden SSH:
- Disable root login  
- Use SSH keys  
- Change port  

---

## 4.13 Firewalls

### UFW
```
ufw enable
ufw allow 22
```

### FirewallD
```
firewall-cmd --add-port 80/tcp
```

---

## 4.14 System Monitoring Tools

- `top`, `htop`
- `free -h`
- `vmstat`
- `iostat`
- `dstat`

---

## 4.15 Linux Interview Questions

### Q1: Difference between hard link and soft link?
Hard link → same inode  
Soft link → shortcut (symbolic link)

### Q2: What is a process vs thread?
Process = independent program  
Thread = lightweight execution unit inside process

### Q3: How to find high CPU usage?
Use `top` or `ps aux --sort=-%cpu`

### Q4: What is exit code?
0 = success  
Nonzero = error

---



# 5. Networking Fundamentals

## 5.1 What is Networking?
Networking is the communication between systems over a medium using protocols.

### Key Components:
- **IP Addressing**
- **DNS**
- **Routing**
- **Ports**
- **Protocols (TCP/UDP)**
- **Firewalls**
- **Load Balancers**

---

## 5.2 OSI Model (7 Layers)

1. **Physical** (Cables, NICs)
2. **Data Link** (Switches, MAC addresses)
3. **Network** (IP, routing)
4. **Transport** (TCP/UDP)
5. **Session**
6. **Presentation**
7. **Application** (HTTP, DNS)

---

## 5.3 TCP vs UDP
| TCP | UDP |
|-----|-----|
| Reliable | Unreliable |
| Slower | Faster |
| Connection-oriented | Connectionless |
| Used for HTTPS, SSH | Used for DNS, gaming |

---

## 5.4 Common Network Commands
- `ping`
- `curl`
- `wget`
- `ip a`
- `ip r`
- `ss -tuln`
- `netstat`
- `dig`, `nslookup`

---

## 5.5 DNS Concepts
- A record → maps name to IP
- CNAME → alias
- MX → mail
- NS → name server

---

## 5.6 Load Balancers
Types:
- L4 (Transport level)
- L7 (Application level)

Examples:
- AWS ALB, NLB
- NGINX
- HAProxy

---

## 5.7 Firewalls
Control incoming and outgoing traffic.

Tools:
- UFW
- firewallD
- AWS Security Groups
- Network ACLs

---

## 5.8 NAT (Network Address Translation)
Converts private IP ↔ public IP.

---

## 5.9 VPC Fundamentals (AWS Networking Basics)
- VPC
- Subnets (Public/Private)
- Route Tables
- NAT Gateway
- Internet Gateway
- Security Groups
- NACLs

---

# 6. AWS Cloud Deep Dive

## 6.1 Introduction to AWS
Amazon Web Services is the most widely used cloud platform.

AWS provides:
- Compute
- Storage
- Networking
- Databases
- Security
- Monitoring

---

## 6.2 AWS Global Infrastructure
- **Regions**
- **Availability Zones (AZs)**
- **Edge Locations**

---

## 6.3 Compute Services

### EC2 (Elastic Compute Cloud)
Virtual servers in AWS.

Key concepts:
- AMI
- Instance types
- EBS volumes
- Security Groups
- Key pairs
- Auto Scaling

---

## 6.4 Load Balancers
Types:
- **ALB** – HTTP/HTTPS
- **NLB** – TCP/UDP
- **CLB** – Legacy

---

## 6.5 Storage Services

### S3
Object storage used for:
- Backups
- Static websites
- Application assets
- Logging

### EBS
Block storage for EC2.

### EFS
Network file system for multi-instance workloads.

---

## 6.6 Databases
- RDS (MySQL, PostgreSQL, MariaDB)
- DynamoDB (NoSQL)
- Aurora
- ElastiCache (Redis, Memcached)

---

## 6.7 IAM (Identity & Access Management)
Controls access to AWS resources.

Components:
- Users
- Groups
- Roles
- Policies
- MFA

Best practices:
- Least privilege
- No root usage
- Use roles instead of access keys

---

## 6.8 Networking (VPC)

### VPC Components:
- Subnets
- Route Tables
- IGW
- NAT Gateway
- Security Groups
- NACLs

---

## 6.9 Serverless Services

### Lambda
No servers needed, event-driven functions.

### API Gateway
Front-door for APIs.

### SQS / SNS
Messaging & queues for decoupled systems.

---

## 6.10 Monitoring in AWS
- CloudWatch Metrics
- CloudWatch Logs
- CloudWatch Alarms
- CloudTrail (auditing)
- AWS Config (compliance)

---

## 6.11 High Availability Architecture on AWS
A standard production system:

```
Route 53 → ALB → EC2/ECS/EKS (Multi-AZ) → RDS Multi-AZ
```

---

## 6.12 AWS Interview Questions

### Q1: Difference between Security Groups and NACLs?
SG = instance level  
NACL = subnet level

### Q2: What is Auto Scaling?
Automatically adds/removes EC2 instances based on load.

### Q3: What is S3 durability?
99.999999999%

---



# 7. Ansible (Configuration Management)

## 7.1 What is Ansible?
Ansible is an **agentless**, open‑source configuration management and automation tool.  
It uses **SSH** to connect to remote machines and execute tasks defined in **YAML playbooks**.

### Why Ansible?
- Simple, human‑readable syntax  
- No agents required  
- Scales easily  
- Great for provisioning, configuration & orchestration  

---

## 7.2 Ansible Architecture

Components:
- **Control Node** (where Ansible runs)
- **Managed Nodes** (servers being configured)
- **Inventory File** (list of hosts)
- **Modules** (units of work)
- **Playbooks** (YAML automation scripts)
- **Roles** (structured automation)

---

## 7.3 Inventory File Example

```
[web]
192.168.1.10
192.168.1.11

[db]
192.168.1.20
```

---

## 7.4 Ad‑Hoc Commands

```
ansible all -m ping
ansible web -m shell -a "uptime"
```

---

## 7.5 Playbook Example

```yaml
---
- hosts: web
  become: yes
  tasks:
    - name: Install NGINX
      apt:
        name: nginx
        state: present
```

---

## 7.6 Ansible Roles

Directory structure:
```
roles/
  nginx/
    tasks/
    handlers/
    templates/
    vars/
```

---

## 7.7 Ansible Vault

Encrypt sensitive data.

```
ansible-vault encrypt secrets.yml
ansible-vault decrypt secrets.yml
```

---

## 7.8 Use Cases
- Server provisioning  
- Package installation  
- Application deployment  
- Kubernetes cluster setup  
- CI/CD automation  

---

# 8. Terraform (Infrastructure as Code)

## 8.1 What is Terraform?
Terraform is the most popular **declarative Infrastructure as Code (IaC)** tool.

### Why Terraform?
- Cloud‑agnostic  
- Declarative HCL syntax  
- Reusable modules  
- Manages entire infrastructure lifecycle  
- State management  
- Integrates with Kubernetes  

---

## 8.2 Terraform Workflow

```
Write → Plan → Apply → Destroy
```

Commands:
```
terraform init
terraform plan
terraform apply
terraform destroy
```

---

## 8.3 Terraform Configuration Example

```hcl
provider "aws" {
  region = "us-east-1"
}

resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
}
```

---

## 8.4 Variables & Outputs

### variables.tf
```hcl
variable "instance_type" {
  default = "t2.micro"
}
```

### outputs.tf
```hcl
output "instance_ip" {
  value = aws_instance.web.public_ip
}
```

---

## 8.5 Terraform State

Terraform maintains **state** to track resources it manages.

### Remote state backends:
- S3  
- GCS  
- Terraform Cloud  

---

## 8.6 Terraform Modules

Modules help reuse infra code.

Structure:
```
modules/
  vpc/
  ec2/
```

Usage:
```hcl
module "vpc" {
  source = "./modules/vpc"
}
```

---

## 8.7 Common Terraform Resources

- VPC  
- Subnets  
- EC2  
- S3  
- IAM  
- RDS  
- EKS  

---

## 8.8 Terraform + Kubernetes

You can manage Kubernetes objects via Terraform:

```
provider "kubernetes" {}
```

---

## 8.9 Terraform Best Practices
- Use modules  
- Use remote state with locking  
- Run `terraform fmt` and `terraform validate`  
- Do NOT hardcode secrets  
- Use workspaces for environments  

---



# 9. Docker Deep Dive

## 9.1 What is Docker?
Docker is a platform for building, packaging, and running applications inside **containers**.

### Benefits:
- Lightweight  
- Portable  
- Faster development  
- Isolation  
- Works everywhere  

---

## 9.2 Docker Architecture

Components:
- **Docker Engine**
- **Docker Daemon**
- **Docker CLI**
- **Images**
- **Containers**
- **Registries** (Docker Hub, ECR)

---

## 9.3 Dockerfile Example

```Dockerfile
FROM node:18-alpine

WORKDIR /app
COPY package*.json ./
RUN npm install

COPY . .
EXPOSE 3000

CMD ["npm", "start"]
```

---

## 9.4 Common Docker Commands

### Images:
```
docker images
docker build -t app:1 .
docker rmi app:1
```

### Containers:
```
docker run -p 8080:80 nginx
docker ps -a
docker exec -it container sh
docker logs container
docker stop container
```

---

## 9.5 Docker Volumes
Persistent storage outside containers.

```
docker volume create data-vol
docker run -v data-vol:/data alpine
```

---

## 9.6 Docker Networking

Types:
- bridge  
- host  
- overlay  
- none  

Custom network:
```
docker network create app-net
```

---

## 9.7 Multi-Stage Docker Builds

```Dockerfile
FROM golang:1.19 AS build
WORKDIR /src
RUN go build -o app

FROM alpine
COPY --from=build /src/app /app
CMD ["/app"]
```

---

## 9.8 Docker Compose

`docker-compose.yml`

```yaml
version: "3.8"
services:
  web:
    image: nginx
    ports:
      - "8080:80"

  db:
    image: mysql
    environment:
      MYSQL_ROOT_PASSWORD: root
```

---

## 9.9 Image Scanning

Tools:
- Trivy  
- Clair  
- Snyk  

---

# 10. Kubernetes Advanced

## 10.1 Kubernetes Architecture

Control Plane:
- API Server  
- Scheduler  
- Controller Manager  
- etcd  

Worker Nodes:
- kubelet  
- kube-proxy  
- container runtime  

---

## 10.2 Pods, Deployments & ReplicaSets

### Deployment Example:
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: web
spec:
  replicas: 3
  selector:
    matchLabels:
      app: web
  template:
    metadata:
      labels:
        app: web
    spec:
      containers:
        - name: nginx
          image: nginx:latest
```

---

## 10.3 Services (ClusterIP, NodePort, LoadBalancer)

### ClusterIP:
Internal service.

### NodePort:
Exposes port on nodes (range 30000–32767).

### LoadBalancer:
Creates cloud load balancer.

---

## 10.4 Ingress

### Example:
```yaml
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: app-ingress
spec:
  rules:
    - host: app.mydomain.com
      http:
        paths:
          - path: /
            pathType: Prefix
            backend:
              service:
                name: web
                port:
                  number: 80
```

---

## 10.5 ConfigMaps & Secrets

### ConfigMap:
```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: app-config
data:
  APP_ENV: production
```

### Secret:
```yaml
apiVersion: v1
kind: Secret
metadata:
  name: app-secret
data:
  password: cGFzcw==
```

---

## 10.6 Probes

### Liveness:
```yaml
livenessProbe:
  httpGet:
    path: /health
    port: 8080
```

### Readiness:
```yaml
readinessProbe:
  httpGet:
    path: /ready
    port: 8080
```

---

## 10.7 Horizontal Pod Autoscaler (HPA)

```yaml
apiVersion: autoscaling/v2
kind: HorizontalPodAutoscaler
metadata:
  name: web-hpa
spec:
  scaleTargetRef:
    kind: Deployment
    name: web
  minReplicas: 2
  maxReplicas: 10
  metrics:
    - type: Resource
      resource:
        name: cpu
        target:
          type: Utilization
          averageUtilization: 70
```

---

## 10.8 Storage in K8s (PV, PVC, StorageClass)

### PVC Example:
```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: pvc-data
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 5Gi
  storageClassName: gp2
```

---

## 10.9 RBAC

### Role:
```yaml
apiVersion: rbac.authorization.k8s.io/v1
kind: Role
metadata:
  namespace: dev
  name: pod-reader
rules:
  - apiGroups: [""]
    resources: ["pods"]
    verbs: ["get", "list"]
```

---

## 10.10 Network Policies

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

## 10.11 Deployment Strategies

### Rolling Updates (default)  
### Blue-Green  
### Canary (via Argo Rollouts, Istio)

---

## 10.12 Helm Charts

Files:
- Chart.yaml  
- values.yaml  
- templates/  

---

## 10.13 Kubernetes Best Practices

✔ Use probes  
✔ Use HPA  
✔ Use liveness + readiness  
✔ Don’t run root containers  
✔ Use NetworkPolicies  
✔ Use RBAC  
✔ Externalize config  

---



# 9. Docker Deep Dive

## 9.1 What is Docker?
Docker is a platform for developing, shipping, and running applications inside **lightweight, isolated containers**.

---

## 9.2 Docker Architecture
- **Docker Client**
- **Docker Daemon**
- **Images**
- **Containers**
- **Docker Registry (Hub, ECR, GCR)**

---

## 9.3 Dockerfile Basics

Example:
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
CMD ["npm", "start"]
```

---

## 9.4 Image Layers
Each instruction creates a new read-only layer:
- Helps caching  
- Reduces build time  

Run:
```
docker history image_name
```

---

## 9.5 Container Commands
```
docker ps
docker run
docker exec -it
docker stop
docker rm
docker images
docker logs
```

---

## 9.6 Docker Networking
Types:
- bridge
- host
- none
- overlay (Swarm/Kubernetes)

---

## 9.7 Volumes
Persistent storage for containers.

```
docker volume create data
```

Mount:
```
-v data:/var/lib/mysql
```

---

## 9.8 Docker Compose
Multi-container apps.

Example:
```yaml
version: "3"
services:
  web:
    image: nginx
    ports:
      - "80:80"
  db:
    image: mysql
    environment:
      MYSQL_ROOT_PASSWORD: root
```

---

## 9.9 Docker Best Practices
- Use small base images (alpine/distroless)
- Multi-stage builds
- Never store secrets in images
- Tag images properly
- Use healthchecks

---

# 10. Kubernetes Advanced

## 10.1 What is Kubernetes?
A container orchestration platform that manages:
- Scaling
- Deployment
- Load balancing
- Self-healing
- Service discovery

---

## 10.2 Kubernetes Probes

### Liveness Probe
```yaml
livenessProbe:
  httpGet:
    path: /health
    port: 8080
```

### Readiness Probe
```yaml
readinessProbe:
  tcpSocket:
    port: 3306
```

### Startup Probe
For slow-start apps.

---

## 10.3 Autoscaling

### HPA (Horizontal Pod Autoscaler)
```yaml
apiVersion: autoscaling/v2
kind: HorizontalPodAutoscaler
spec:
  minReplicas: 2
  maxReplicas: 10
```

---

## 10.4 Kubernetes Storage

### PVC Example:
```yaml
apiVersion: v1
kind: PersistentVolumeClaim
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 5Gi
```

---

## 10.5 Kubernetes Services (Advanced)

- **ClusterIP**
- **NodePort**
- **LoadBalancer**
- **ExternalName**

---

## 10.6 Ingress Controller

Example:
```yaml
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: app-ingress
```

---

## 10.7 ConfigMaps & Secrets

### ConfigMap:
```yaml
env:
  - name: PORT
    valueFrom:
      configMapKeyRef:
        name: app-config
        key: port
```

### Secret:
```yaml
data:
  password: cGFzc3dvcmQ=
```

---

## 10.8 Security (RBAC)

Role Example:
```yaml
kind: Role
rules:
  - apiGroups: [""]
    resources: ["pods"]
    verbs: ["get", "list"]
```

---

## 10.9 Affinity

Node affinity:
```yaml
nodeAffinity:
  requiredDuringSchedulingIgnoredDuringExecution:
    nodeSelectorTerms:
      - matchExpressions:
          - key: environment
            operator: In
            values: ["prod"]
```

---

## 10.10 Jobs & CronJobs

CronJob example:
```yaml
schedule: "0 0 * * *"
```

---

## 10.11 Deployment Strategies
- Rolling updates  
- Blue/Green  
- Canary  

---

## 10.12 Helm (Advanced)

Chart structure:
```
Chart.yaml
values.yaml
templates/
```

---

## 10.13 Kubernetes Best Practices
- Use probes  
- Limit resources  
- Use namespaces  
- Avoid running containers as root  
- Implement NetworkPolicies  

---



# 11. Monitoring & Logging (Prometheus, Grafana, CloudWatch, EFK)

## 11.1 What is Observability?
Observability = ability to understand system health using:
- **Metrics**
- **Logs**
- **Traces**

---

## 11.2 Prometheus (Metrics Collection)
Prometheus uses **pull-based** scraping.

### Key Components:
- Prometheus Server  
- Exporters  
- Alertmanager  
- Grafana (visualization)  

### Prometheus Scrape Example:
```yaml
scrape_configs:
  - job_name: "node"
    static_configs:
      - targets: ["10.0.1.10:9100"]
```

---

## 11.3 Grafana
Used to visualize metrics from Prometheus, CloudWatch, Loki, etc.

Common dashboards:
- Node CPU/Memory
- Pod states
- HTTP latency
- DB performance

---

## 11.4 Exporters
- Node Exporter (system metrics)
- Kube-State-Metrics (K8s objects)
- Blackbox Exporter (ping/HTTP checks)

---

## 11.5 Alertmanager
Prometheus alerting system.

Alerts sent to:
- Slack
- Email
- PagerDuty
- Webhooks

---

## 11.6 EFK Stack (Logging)
EFK = Elasticsearch + Fluentd + Kibana

### Flow:
Pods → Fluentd → Elasticsearch → Kibana

---

## 11.7 CloudWatch (AWS Monitoring)
CloudWatch provides:
- Metrics
- Logs
- Events
- Alarms

Used widely in AWS deployments.

---

## 11.8 Golden Signals (SRE)
1. Latency  
2. Traffic  
3. Errors  
4. Saturation  

---

## 11.9 Distributed Tracing
Tools:
- Jaeger
- OpenTelemetry

Useful in microservices to trace request flows.

---

## 11.10 Monitoring Best Practices
- Monitor everything (infra + app)
- Alerts must be actionable
- Avoid alert fatigue
- Build dashboards for visibility

---

# 12. DevSecOps (Security in DevOps Pipelines)

## 12.1 What is DevSecOps?
DevSecOps integrates security at every stage of CI/CD.

---

## 12.2 Security Scanning Types

### SAST (Static Analysis)
Scans source code.
- SonarQube
- Checkmarx

### SCA (Dependency Scanning)
Checks vulnerable libraries.
- Snyk
- Trivy

### DAST (Runtime Scanning)
Tests running applications.

---

## 12.3 Container Image Scanning
Using Trivy:
```
trivy image myapp:latest
```

---

## 12.4 IaC Scanning
Tools:
- Checkov
- Terrascan
- TFSec

Command:
```
checkov -d .
```

---

## 12.5 Secrets Management
Tools:
- HashiCorp Vault  
- AWS Secrets Manager  
- SSM Parameter Store  

Never store secrets in:
- Git
- Dockerfiles
- Terraform variables

---

## 12.6 CI/CD Pipeline Security
- Use OIDC instead of access keys  
- Rotate secrets regularly  
- Restrict runners/agents  
- Scan every build  

---

## 12.7 Kubernetes Security
- RBAC  
- NetworkPolicies  
- PodSecurityStandards  
- Non-root containers  
- readOnlyRootFilesystem: true  

---

## 12.8 Cloud Security Basics (AWS)
- IAM least privilege  
- MFA required  
- No root key usage  
- S3 bucket encryption  
- GuardDuty enabled  
- CloudTrail for auditing  

---

## 12.9 DevSecOps Best Practices
- Automate all scans  
- Encrypt data at rest & transit  
- Secure supply chain  
- Use signed container images  
- Detect drift in infrastructure  

---



# DevOps Handbook – Part 2 (Chapters 13–17)


# 13. Cloud Architecture & Microservices

## 13.1 High Availability (HA)
High Availability ensures uninterrupted service even during failures.

### Strategies:
- Deploy across multiple Availability Zones (AZs)
- Use Load Balancers (ALB/NLB)
- Implement Auto Scaling Groups
- Build redundancy for critical components
- Continuous health checks

---

## 13.2 Scalability

### Vertical Scaling:
Increasing server resources (CPU/RAM).  
Example: t2.micro → t3.large

### Horizontal Scaling:
Adding more servers/pods.  
Examples:
- AWS Auto Scaling Groups
- Kubernetes Horizontal Pod Autoscaler (HPA)

---

## 13.3 Disaster Recovery (DR)

### Key Concepts:
- **RTO** (Recovery Time Objective)
- **RPO** (Recovery Point Objective)

### DR Models:
1. Backup & Restore  
2. Pilot Light  
3. Warm Standby  
4. Multi-Region Active-Active (zero downtime)

---

## 13.4 Microservices Architecture
Microservices split applications into independent components.

### Benefits:
- Independent deployment
- Smaller, manageable codebases
- Fault isolation
- Independent scaling

### Challenges:
- Distributed logging
- Complex networking
- Observability
- Service discovery

---

## 13.5 API Gateway
Acts as a single entry point for all client requests.

### Responsibilities:
- Routing
- Authentication & authorization
- Rate limiting
- SSL termination
- Centralized logging

### Tools:
- AWS API Gateway
- Kong
- NGINX
- Istio Ingress Gateway

---

## 13.6 Service Discovery
Allows services with dynamic IPs to find each other.

### Examples:
- Kubernetes DNS
- Consul
- Eureka
- AWS Cloud Map

---

## 13.7 Message Queues
Enable asynchronous communication.

### Tools:
- Kafka
- RabbitMQ
- AWS SQS

### Benefits:
- Decoupling
- Buffers peak traffic
- Fault tolerance

---

## 13.8 Event-Driven Architecture
Uses events to trigger actions across systems.

### Examples:
- S3 triggers Lambda
- SNS broadcasting messages
- Kafka streaming data pipelines

---

## 13.9 Serverless Architecture
Runs code without managing servers.

### AWS Lambda benefits:
- Auto-scaling
- Pay-per-use
- Event-driven execution
- Reduced operational overhead

---

## 13.10 Caching Layer
Improves performance & reduces database load.

### Tools:
- Redis
- Memcached
- CloudFront (CDN)

---

## 13.11 Deployment Patterns

### Blue/Green:
Two environments:
- Blue = current version
- Green = new version  
Switch traffic instantly.

### Rolling Updates:
Gradually replace pods/instances.

### Canary Releases:
Release new version to small traffic % first.

---

## 13.12 Cloud Architecture Example

```
User → Route53 → ALB → ECS/EKS/EC2 ASG (Multi-AZ)
                        ↓
                     RDS Multi-AZ
                        ↓
                     Redis Cache
                        ↓
                     S3 Storage
```

---

## 13.13 Best Practices
- Use Multi-AZ deployments
- Encrypt data in transit & at rest
- Apply least privilege IAM
- Implement centralized logging (EFK/Loki)
- Enable autoscaling where possible
- Use Infrastructure as Code (Terraform)


# 14. CI/CD Pipelines

## 14.1 What is CI/CD?
CI/CD automates the entire software delivery lifecycle:
- **Continuous Integration (CI):** Automates building, testing, and merging code.
- **Continuous Delivery (CD):** Automatically prepares releases for deployment.
- **Continuous Deployment:** Fully automated deployment to production.

---

## 14.2 Benefits of CI/CD
- Faster releases  
- Improved software quality  
- Reduced manual effort  
- Smaller, safer changes  
- Faster feedback loops  

---

## 14.3 Jenkins (CI/CD Automation)
Jenkins is one of the most widely used CI/CD tools.

### Key Features:
- Pipelines-as-code (Jenkinsfile)
- Plugins for integration
- Declarative and scripted pipelines
- Supports Docker, Kubernetes, AWS, GitHub

### Example Jenkinsfile (Declarative Pipeline):
```groovy
pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
    stage('Docker Build') {
      steps {
        sh 'docker build -t myapp .'
      }
    }
    stage('Deploy to Kubernetes') {
      steps {
        sh 'kubectl apply -f k8s/'
      }
    }
  }
}
```

---

## 14.4 GitHub Actions (CI/CD)
GitHub Actions provides native GitHub automation using YAML workflows.

### Example:
```yaml
name: CI Pipeline

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: npm install
      - run: npm test
```

---

## 14.5 GitLab CI/CD
GitLab provides fully integrated CI/CD with Runners.

### Example:
```yaml
stages:
  - build
  - test
  - deploy

build-job:
  stage: build
  script:
    - mvn package
```

---

## 14.6 Deployment Strategies

### Rolling Deployment
Replace pods gradually with zero downtime.

### Blue-Green Deployment
Two live environments:
- Blue (current)
- Green (new version)

### Canary Deployment
Release new version to small % traffic first.

---

## 14.7 GitOps (ArgoCD)
Git is the single source of truth for deployments.

### ArgoCD Capabilities:
- Auto-sync changes
- Rollback support
- Deployment visual dashboard

---

## 14.8 CI/CD Best Practices
- Every commit triggers CI
- Automate tests (unit, integration)
- Use environment-specific configs
- Store secrets securely (Vault/KMS)
- Implement SAST + SCA scanning
- Use Infrastructure as Code for deployments
- Use short-lived tokens instead of static credentials

---



# 15. Soft Skills, SRE Concepts & DevOps Interview Preparation

## 15.1 Essential Soft Skills for DevOps Engineers
DevOps engineers must combine technical excellence with strong communication and collaboration.

### Key Soft Skills:
- **Problem-Solving:** Break down complex issues logically.
- **Communication:** Explain infra concepts clearly to devs, ops, managers.
- **Collaboration:** Work across Dev, QA, Security, Cloud teams.
- **Adaptability:** Tools and platforms evolve constantly.
- **Ownership:** Take responsibility for deployments and incidents.
- **Time Management:** Prioritize critical tasks effectively.
- **Calm Under Pressure:** Essential during production incidents.
- **Documentation:** Clear runbooks, SOPs, troubleshooting guides.

---

## 15.2 SRE (Site Reliability Engineering)
SRE extends DevOps with reliability engineering principles.

### Core Ideas:
- Reduce toil through automation  
- Track SLOs and error budgets  
- Standardize operations  
- Create predictable deployments  
- Improve observability and reliability  

---

## 15.3 SLIs, SLOs, SLAs

### SLI – Service Level Indicator
A metric that measures performance:
- Latency
- Error rate
- Availability

### SLO – Service Level Objective
Internal performance target:
- 99.9% uptime  
- <200ms p95 latency  

### SLA – Service Level Agreement
Contract with customers defining:
- Penalties for downtime  
- Service expectations  

---

## 15.4 Incident Management

### Incident Lifecycle:
1. **Detection**
2. **Acknowledgement**
3. **Mitigation**
4. **Resolution**
5. **RCA (Root Cause Analysis)**
6. **Action Items**
7. **Prevention**

### Common Triggers:
- CPU/memory spikes
- High 5xx errors
- Node/pod failures
- DB deadlocks
- Disk full
- Network issues

---

## 15.5 Troubleshooting Framework
Follow a structured workflow:

1. Identify scope  
2. Check logs  
3. Check metrics  
4. Check recent changes  
5. Test hypotheses  
6. Validate and resolve  
7. Document findings  

### Common Scenarios:
- Pod crashloop → check events + logs  
- Server unreachable → SG/NACL/route table  
- App slow → DB queries + CPU/memory  

---

## 15.6 Behavioral Interview Preparation

### Common Questions:
- “Tell me about yourself.”
- “Describe an incident you handled.”
- “How do you resolve conflicts?”
- “What is your biggest failure and what did you learn?”

### Tips:
- Use STAR format  
- Show ownership  
- Demonstrate learning  
- Show calm and methodical thinking  

---

## 15.7 Technical Interview Preparation

### Topics Interviewers Focus On:
- Linux commands & scripting
- Git & branching strategies
- Docker & Kubernetes
- Jenkins pipelines
- Terraform & IaC
- AWS core services
- Networking concepts
- Monitoring & logging stack
- Security fundamentals

---

## 15.8 Resume Tips for DevOps Engineers
- Showcase real projects
- Highlight automation achievements
- Use metrics (e.g., “reduced deploy time by 60%”)
- Include cloud, container, IaC tools
- Keep resume concise (1–2 pages)
- Include certifications (AWS, Kubernetes, Terraform)

---

## 15.9 DevOps Mindset
- Automate everything repetitive  
- Fix root causes, not symptoms  
- Use blameless communication  
- Always monitor performance  
- Continuously learn new tools  
- Prioritize reliability and security  

---



# 16. Complete DevOps Learning Roadmap (Beginner → Pro)

This roadmap guides you from absolute beginner to production-ready DevOps engineer.

---

## 16.1 Phase 1 — Foundations (1–2 Months)

### Linux Essentials
- Commands (ls, cd, ps, top, grep)
- File permissions & ownership
- Processes & services
- Shell scripting
- Cron jobs
- SSH & key-based authentication

### Git & GitHub
- Branching, merging, rebasing
- Pull requests
- Git workflows (GitFlow)
- Handling merge conflicts

### Projects:
- Automated backup script  
- Cron-based monitoring script  
- GitHub project with feature branches  

---

## 16.2 Phase 2 — Core DevOps Tools (2 Months)

### Docker
- Dockerfile
- Images & layers
- Volumes & networks
- Docker Compose

### Kubernetes
- Pods, Deployments, Services
- Ingress
- ConfigMaps, Secrets
- StatefulSets
- HPA (Autoscaling)

### CI/CD Basics
- Jenkins pipelines
- GitHub Actions workflows

### Projects:
- Dockerize an app  
- Multi-container setup with Compose  
- Deploy app to Kubernetes locally  

---

## 16.3 Phase 3 — Cloud & Infrastructure (2–3 Months)

### AWS Services
- EC2, VPC, Subnets, Routing
- ALB/NLB
- S3, EBS, EFS
- IAM roles & policies
- RDS
- CloudWatch
- Lambda & API Gateway

### Projects:
- VPC creation  
- Deploy 3-tier application  
- AWS serverless application  
- Multi-AZ deployment setup  

---

## 16.4 Phase 4 — Infrastructure as Code (1–2 Months)

### Terraform
- Providers
- Resources
- Modules
- Remote state
- Workspaces

### Ansible
- Playbooks
- Templates
- Roles
- Vault

### Projects:
- VPC using Terraform  
- EC2 + ALB deployment via Terraform  
- Server provisioning with Ansible  

---

## 16.5 Phase 5 — Advanced DevOps (2 Months)

### Monitoring & Observability
- Prometheus + Grafana
- Node Exporter
- Alertmanager
- CloudWatch dashboards

### DevSecOps
- Static scanning (SonarQube)
- Image scanning (Trivy)
- IaC scanning (Checkov)
- Secrets management (Vault)

### GitOps
- ArgoCD deployments
- Auto-sync & rollback setup

### Projects:
- K8s monitoring stack  
- Complete DevSecOps pipeline  
- GitOps workflow with ArgoCD  

---

## 16.6 Phase 6 — System Design & SRE (Ongoing)

Focus on:
- Microservices architecture
- High availability / scalability
- SLIs, SLOs, SLAs
- Error budgets
- Incident response
- Distributed tracing

---

## 16.7 Daily Learning Plan

### Beginner (0–3 months)
- Linux: 2 hrs  
- Git: 1 hr  
- Docker/K8s: 2 hrs  

### Intermediate (3–7 months)
- AWS: 3 hrs  
- Terraform: 1 hr  
- Jenkins: 2 hrs  

### Advanced (7–12 months)
- Monitoring: 2 hrs  
- DevSecOps: 1 hr  
- Architecture: 2 hrs  

---

## 16.8 Roadmap Summary

| Phase | Duration |
|-------|----------|
| Foundations | 1–2 months |
| Core Tools | 2 months |
| Cloud & Infra | 2–3 months |
| IaC | 1–2 months |
| Advanced DevOps | 2 months |
| SRE & Design | Continuous |

---



# 17. Real DevOps Projects (Beginner → Advanced → Production)

Real projects demonstrate practical skills and make your resume stand out.  
This chapter lists industry-aligned projects you can build to reach production-level competency.

---

# 17.1 Beginner Projects

## Project 1 — Dockerize a Simple Application
**Skills:** Docker, Dockerfile, Container basics  
**Tasks:**
- Create Dockerfile  
- Build & run image  
- Push image to Docker Hub  

---

## Project 2 — CI Pipeline Using GitHub Actions
**Skills:** GitHub Actions, CI  
**Tasks:**
- Configure YAML workflow  
- Automate tests & build  
- Trigger pipeline on push  

---

## Project 3 — Monitoring Script with Cron
**Skills:** Bash, Cron, Linux automation  
**Tasks:**
- Monitor CPU/RAM  
- Send alert on threshold  
- Run every minute/hour via cron  

---

# 17.2 Intermediate Projects

## Project 4 — Multi-Container App Using Docker Compose
**Skills:** Compose, Networking, Volumes  
**Tasks:**
- Define frontend, backend, DB  
- Network containers  
- Persist DB data  

---

## Project 5 — Jenkins CI/CD Pipeline
**Skills:** Jenkinsfile, CI/CD, Docker  
**Tasks:**
- Build → Test → Dockerize → Push  
- Add credential bindings  
- Automate full pipeline  

---

## Project 6 — Deploy to Kubernetes (Minikube or K3s)
**Skills:** K8s, YAML, Ingress  
**Tasks:**
- Create deployments & services  
- Use ConfigMaps & Secrets  
- Add Ingress Controller  

---

## Project 7 — AWS VPC Using Terraform
**Skills:** Terraform, AWS networking  
**Tasks:**
- Create VPC, Subnets, Routing  
- Launch EC2 instance  
- Use remote state (S3 + DynamoDB)  

---

# 17.3 Advanced Projects

## Project 8 — Full CI/CD: GitHub → Jenkins → Docker → ECR → EKS
**Skills:** Full pipeline automation  
**Flow:**
- GitHub push → Jenkins → Build → Push → Deploy  
- Deploy app to AWS EKS  

---

## Project 9 — Monitoring Stack: Prometheus + Grafana
**Skills:** Observability  
**Tasks:**
- Deploy Prometheus & Grafana on K8s  
- Configure Node Exporter  
- Build dashboards  

---

## Project 10 — EFK Logging Stack
**Skills:** Logging & search  
**Tasks:**
- Deploy Elasticsearch  
- Configure Fluentd DaemonSet  
- Visualize logs in Kibana  

---

## Project 11 — GitOps with ArgoCD
**Skills:** GitOps, K8s automation  
**Tasks:**
- Configure app repo  
- Auto-sync deployments  
- Implement rollbacks  

---

# 17.4 Production-Level Projects

## Project 12 — Multi-AZ Highly Available Architecture (AWS)
**Skills:** Cloud architecture  
**Tasks:**
- VPC + Multi-AZ subnets  
- ALB + ASG  
- RDS Multi-AZ  
- Redis cache  
- Route53 failover  

---

## Project 13 — Secure DevOps Pipeline (DevSecOps)
**Skills:** Security automation  
**Includes:**
- Trivy image scan  
- Checkov IaC scan  
- SonarQube static analysis  
- Secret scanning  
- KMS encryption  

---

## Project 14 — Distributed Microservices on Kubernetes
**Skills:** Microservices, autoscaling  
**Tasks:**
- Deploy multiple services  
- Add message queue (Kafka/SQS)  
- Implement HPA  
- Add distributed tracing (Jaeger)  

---

# 17.5 Bonus Projects

- Service Mesh with Istio  
- Serverless App using Lambda  
- Global CDN using CloudFront  
- Automated cost monitoring system  
- Kubernetes operators  

---

# 17.6 Recommended Projects for Resume

If you include only the strongest projects, choose:
1. Full CI/CD Pipeline to EKS  
2. Terraform VPC + EKS provisioning  
3. Prometheus + Grafana Monitoring  
4. EFK Logging stack  
5. GitOps with ArgoCD  

These are highly valued in interviews and represent real-world production experience.

---

