# 🚀 My DevOps Learning Roadmap (6 Months)
> Backend Engineer → Senior DevOps Engineer
> 
> **Track my progress here — update checkboxes as I go.**

---

## 🎯 End Goal

By the end of 6 months, I will be able to:

- [ ] Containerize real applications
- [ ] Build production CI/CD pipelines
- [ ] Deploy to Kubernetes clusters
- [ ] Manage infrastructure with Terraform
- [ ] Monitor systems with Prometheus + Grafana
- [ ] Automate ops with Bash/Python/Ansible
- [ ] Secure pipelines and clusters
- [ ] Troubleshoot production incidents
- [ ] Build a portfolio that gets interviews
- [ ] Think like a Senior DevOps Engineer

---

## 📌 Core Philosophy

> **70% Hands-on | 20% Architecture understanding | 10% Reading docs**

---

## 📦 Projects I Will Build

| # | Project | Status |
|---|---------|--------|
| 1 | Dockerized backend platform | ⬜ Not started |
| 2 | Jenkins CI/CD pipeline | ⬜ Not started |
| 3 | Kubernetes microservice deployment | ⬜ Not started |
| 4 | Terraform cloud infrastructure | ⬜ Not started |
| 5 | Monitoring stack (Prometheus + Grafana) | ⬜ Not started |
| 6 | Full production SaaS platform | ⬜ Not started |

---

## 📅 Month 1 — Linux, Networking, Git, Docker

> **Objective:** Become dangerous on the terminal and understand how apps run.

### Week 1 — Linux Like a Real Engineer

**Topics:**
- [ ] File system
- [ ] Permissions
- [ ] Processes
- [ ] Users/groups
- [ ] SSH
- [ ] Services (`systemctl`)
- [ ] Logs
- [ ] Cron jobs
- [ ] Environment variables

**Practice:**
- [ ] Create users
- [ ] Kill stuck processes
- [ ] Inspect logs
- [ ] Configure SSH keys
- [ ] Run background services

**✅ Deliverable:** Build my own Linux cheat sheet

---

### Week 2 — Networking for DevOps

**Topics:**
- [ ] DNS
- [ ] HTTP/HTTPS
- [ ] TCP vs UDP
- [ ] Ports
- [ ] Reverse proxy
- [ ] Load balancer
- [ ] Firewall
- [ ] NAT

**Practice:**
- [ ] Use `curl`
- [ ] Use `netstat` / `ss`
- [ ] Inspect requests
- [ ] Configure Nginx reverse proxy

**✅ Deliverable:** Deploy Spring Boot behind Nginx

---

### Week 3 — Git Advanced

**Topics:**
- [ ] Rebase
- [ ] Cherry-pick
- [ ] Tags
- [ ] Release strategy
- [ ] Branching models
- [ ] Conflict resolution

**Practice:**
- [ ] Simulate team workflows
- [ ] Recover bad commits
- [ ] Create releases

---

### Week 4 — Docker Mastery

**Topics:**
- [ ] Images & containers
- [ ] Layers
- [ ] Networks & Volumes
- [ ] Multi-stage builds
- [ ] Docker Compose
- [ ] Registry

**Practice:** Containerize Spring Boot + PostgreSQL + Redis

**✅ Deliverable:** Full backend stack running with Docker Compose

---

## 📅 Month 2 — CI/CD Engineering

> **Objective:** Automate build, test, release, deploy.

### Week 5 — CI/CD Concepts

- [ ] Pipeline stages
- [ ] Build artifacts
- [ ] Test automation
- [ ] Deployment strategies
- [ ] Rollback
- [ ] Secrets management

---

### Week 6 — Jenkins

- [ ] Jenkins setup
- [ ] Agents
- [ ] Pipelines as code
- [ ] Shared libraries
- [ ] Credentials

**Practice:** Pipeline for Spring Boot (Build → Test → Package → Dockerize → Push image)

---

### Week 7 — GitHub Actions / GitLab CI

- [ ] Learn modern CI/CD alternatives
- [ ] Rebuild same pipeline using GitHub Actions

---

### Week 8 — Deployment Strategies

- [ ] Blue/Green
- [ ] Canary
- [ ] Rolling updates
- [ ] Zero downtime deploys

**✅ Deliverable:** Complete CI/CD pipeline deploying backend automatically

---

## 📅 Month 3 — Kubernetes Deep Mastery

> **Objective:** Become productive with K8s, not scared of it.

### Week 9 — Kubernetes Core

- [ ] Pods
- [ ] Deployments
- [ ] Services
- [ ] Namespaces
- [ ] ConfigMaps
- [ ] Secrets

**Practice:** Deploy backend app

---

### Week 10 — Advanced Kubernetes

- [ ] Ingress
- [ ] Persistent Volumes
- [ ] HPA (Horizontal Pod Autoscaler)
- [ ] Resource limits
- [ ] Probes
- [ ] Init containers

**Practice:** Production-ready deployment

---

### Week 11 — Helm

- [ ] Charts
- [ ] Values
- [ ] Templates
- [ ] Releases

**Practice:** Package backend as Helm chart

---

### Week 12 — Troubleshooting Kubernetes

- [ ] CrashLoopBackOff
- [ ] Pending pods
- [ ] DNS failures
- [ ] Logs & `kubectl debug`

**✅ Deliverable:** Deploy microservice stack on Kubernetes

---

## 📅 Month 4 — Cloud + Infrastructure as Code

> **Objective:** Provision real infrastructure professionally.

### Week 13 — AWS Fundamentals

- [ ] IAM
- [ ] EC2
- [ ] VPC
- [ ] Security Groups
- [ ] S3
- [ ] RDS
- [ ] ECR
- [ ] Load Balancer

---

### Week 14 — Terraform Basics

- [ ] Providers
- [ ] Resources
- [ ] Variables & Outputs
- [ ] State

**Practice:** Create VPC + EC2 + Security Groups

---

### Week 15 — Terraform Advanced

- [ ] Modules
- [ ] Remote state
- [ ] Workspaces
- [ ] CI integration

**Practice:** Provision complete backend environment

---

### Week 16 — Kubernetes on Cloud

- [ ] EKS / AKS / GKE concepts

**✅ Deliverable:** Deploy app to cloud Kubernetes cluster

---

## 📅 Month 5 — Monitoring, Logging, Reliability

> **Objective:** Operate systems in production.

### Week 17 — Prometheus

- [ ] Metrics
- [ ] Exporters
- [ ] Alerts
- [ ] Scraping

**Practice:** Monitor Spring Boot app

---

### Week 18 — Grafana

- [ ] Dashboards
- [ ] Alerts
- [ ] Panels
- [ ] SLO charts

**✅ Deliverable:** Executive dashboard

---

### Week 19 — Logging Stack

- [ ] ELK / OpenSearch
- [ ] Loki
- [ ] Structured logs
- [ ] Correlation IDs

**Practice:** Centralize app logs

---

### Week 20 — Reliability Engineering

- [ ] SLI / SLO / SLA
- [ ] Incident response
- [ ] Root cause analysis
- [ ] Capacity planning

**✅ Deliverable:** Full observability stack for backend system

---

## 📅 Month 6 — Security, Automation, Real Projects, Interview Prep

> **Objective:** Become hireable.

### Week 21 — DevSecOps

- [ ] Secrets scanning
- [ ] Dependency scanning
- [ ] Container scanning
- [ ] RBAC
- [ ] Policy enforcement

**Tools:** Trivy, SonarQube, Snyk (optional)

---

### Week 22 — Automation with Bash + Python + Ansible

- [ ] Bash scripting
- [ ] Python automation
- [ ] Ansible playbooks

**Practice:** Automate deployments

---

### Week 23 — Real Production Project

Build a full SaaS backend platform from scratch:

- [ ] Spring Boot APIs
- [ ] PostgreSQL
- [ ] Redis
- [ ] Docker
- [ ] CI/CD
- [ ] Kubernetes
- [ ] Monitoring
- [ ] Terraform
- [ ] Alerts
- [ ] Secure secrets

---

### Week 24 — Interview + Portfolio

- [ ] Resume updated
- [ ] GitHub portfolio ready
- [ ] DevOps interview questions practiced
- [ ] System design scenarios practiced
- [ ] Troubleshooting scenarios practiced

---

## 📚 Resources

| Topic | Resource |
|-------|----------|
| Kubernetes | [TechWorld with Nana](https://www.techworld-with-nana.com/devops-bootcamp) |
| Kubernetes labs | KodeKloud |
| CI/CD | [Nana GitLab CI/CD](https://www.techworld-with-nana.com/gitlab-cicd-course) |
| Jenkins | Jenkins official docs |
| Terraform | HashiCorp Learn |
| Monitoring | Prometheus docs + Grafana labs |
| Ansible | Jeff Geerling community |

---

## 💡 My Advantage as a Backend Engineer

I already understand APIs, deployment pain, logs, debugging, databases, architecture, and shipping software. This means I can excel at:

- Release engineering
- Platform engineering
- CI/CD
- Kubernetes app operations
- Production debugging
- Cloud backend systems

> I am not starting from zero.

---

## 📊 Overall Progress

| Month | Focus | Status |
|-------|-------|--------|
| Month 1 | Linux, Networking, Git, Docker | ⬜ Not started |
| Month 2 | CI/CD Engineering | ⬜ Not started |
| Month 3 | Kubernetes | ⬜ Not started |
| Month 4 | Cloud + Terraform | ⬜ Not started |
| Month 5 | Monitoring + Reliability | ⬜ Not started |
| Month 6 | Security + Portfolio + Jobs | ⬜ Not started |

---

*Started: ___________  |  Target end date: ___________*
