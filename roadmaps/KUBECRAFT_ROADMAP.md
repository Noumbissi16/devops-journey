# ☸️ My Free KubeCraft Roadmap (6 Months)
> Backend Engineer → Real Kubernetes + DevOps Engineer
>
> **Rules: 1–2 hrs/day minimum | Build every week | Post progress publicly | Deploy real apps**

---

## 📊 Overall Progress

| Phase | Focus | Weeks | Status |
|-------|-------|-------|--------|
| Phase 0 | Lab Setup | Week 0 | ⬜ Not started |
| Phase 1 | Linux + Networking | Weeks 1–4 | ⬜ Not started |
| Phase 2 | Git + GitHub + Automation | Weeks 5–6 | ⬜ Not started |
| Phase 3 | Docker Mastery | Weeks 7–10 | ⬜ Not started |
| Phase 4 | Kubernetes Core | Weeks 11–16 | ⬜ Not started |
| Phase 5 | Kubernetes Advanced | Weeks 17–20 | ⬜ Not started |
| Phase 6 | CI/CD + GitOps | Weeks 21–24 | ⬜ Not started |
| Phase 7 | Monitoring + Logging | Weeks 25–26 | ⬜ Not started |
| Phase 8 | Security | Weeks 27–28 | ⬜ Not started |
| Phase 9 | Cloud Kubernetes | Weeks 29–32 | ⬜ Not started |
| Phase 10 | Real Portfolio Projects | Weeks 33–36 | ⬜ Not started |

---

## 🔧 Phase 0 (Week 0) — Setup My DevOps Lab

### Install
- [ ] Ubuntu VM or dual boot
- [ ] VS Code
- [ ] Git
- [ ] Docker
- [ ] Minikube or Kind
- [ ] kubectl
- [ ] Postman
- [ ] Helm *(later)*

### Create Accounts
- [ ] GitHub
- [ ] Docker Hub
- [ ] AWS / GCP free tier *(later)*
- [ ] LinkedIn

### ✅ Deliverable
- [ ] Create GitHub repo named `devops-journey` and document everything

---

## 🐧 Phase 1 (Weeks 1–4) — Linux + Networking Foundations

> Strong Kubernetes engineers are strong Linux engineers first. Don't skip this.

### Linux
- [ ] `pwd`, `ls`, `cd`
- [ ] `cp`, `mv`, `rm`
- [ ] `cat`, `grep`, `sed`, `awk`
- [ ] `chmod`, `chown`
- [ ] `ps`, `top`, `kill`
- [ ] `systemctl`
- [ ] `journalctl`
- [ ] `apt`

### Networking
- [ ] IP
- [ ] DNS
- [ ] Ports
- [ ] HTTP/HTTPS
- [ ] TCP vs UDP
- [ ] Reverse proxy
- [ ] SSH

### Weekly Project
- [ ] Deploy a Java Spring Boot app manually on Ubuntu

### ✅ Deliverables
- [ ] Linux cheat sheet
- [ ] Blog post: "50 Linux Commands I Learned"
- [ ] App hosted locally

---

## 🌿 Phase 2 (Weeks 5–6) — Git + GitHub + Automation

### Git
- [ ] `init`, `clone`
- [ ] `branch`, `merge`, `rebase`
- [ ] PR workflow
- [ ] Tags & release strategy

### Automation
- [ ] Bash scripts (`.sh` files)
- [ ] Cron jobs

### Weekly Project
- [ ] Create deployment script:
```bash
git pull
mvn clean package
java -jar app.jar
```

### ✅ Deliverables
- [ ] Automated deployment script
- [ ] GitHub README with badges
- [ ] Clean commit history

---

## 🐳 Phase 3 (Weeks 7–10) — Docker Mastery

### Topics
- [ ] Images & Containers
- [ ] Volumes & Networks
- [ ] Dockerfile
- [ ] Multi-stage builds
- [ ] Docker Compose

### Projects
- [ ] **Project 1:** Containerize Spring Boot API
- [ ] **Project 2:** Multi-container stack (Spring Boot + PostgreSQL + Redis + Nginx)

### ✅ Deliverables
- [ ] Push images to Docker Hub
- [ ] README with architecture diagram

---

## ☸️ Phase 4 (Weeks 11–16) — Kubernetes Core

> This is the heart of the roadmap.

### Core Objects
- [ ] Cluster & Node
- [ ] Pod
- [ ] ReplicaSet
- [ ] Deployment
- [ ] Service
- [ ] Namespace
- [ ] ConfigMap & Secret

### Practice Commands
- [ ] `kubectl get pods`
- [ ] `kubectl describe pod`
- [ ] `kubectl logs`
- [ ] `kubectl exec -it`
- [ ] `kubectl apply -f`
- [ ] `kubectl delete -f`

### YAML Skills
- [ ] Learn manifests deeply

### Project
- [ ] Deploy Spring Boot API to Minikube

### ✅ Deliverables
- [ ] Full manifests repo
- [ ] App accessible in cluster
- [ ] Troubleshooting notes

---

## ⚙️ Phase 5 (Weeks 17–20) — Kubernetes Advanced

> Most learners stop at Pods/Deployments. Don't.

### Topics
- [ ] Ingress
- [ ] Persistent Volumes
- [ ] StatefulSets
- [ ] Jobs / CronJobs
- [ ] HPA Autoscaling
- [ ] RBAC
- [ ] Resource requests/limits
- [ ] Liveness probe
- [ ] Readiness probe

### Project
- [ ] Production-like e-commerce backend on Kubernetes

### ✅ Deliverables
- [ ] Ingress routing working
- [ ] Autoscaling demo
- [ ] Persistent database volume

---

## 🔄 Phase 6 (Weeks 21–24) — CI/CD + GitOps

### CI/CD Concepts
- [ ] Pipelines (Build → Test → Deploy)
- [ ] Environments
- [ ] Rollbacks

### Tools — pick one first
- [ ] GitHub Actions
- [ ] GitLab CI
- [ ] Jenkins

### GitOps
- [ ] ArgoCD

### Project
- [ ] Push to GitHub → Auto deploy to Kubernetes

### ✅ Deliverables
- [ ] CI pipeline screenshots
- [ ] Auto deploy working
- [ ] Rollback strategy documented

---

## 📊 Phase 7 (Weeks 25–26) — Monitoring + Logging

### Topics
- [ ] Prometheus
- [ ] Grafana
- [ ] Loki
- [ ] Alerts & Metrics

### Project
- [ ] Observe my Kubernetes cluster

### ✅ Deliverables
- [ ] Dashboards built
- [ ] CPU/memory metrics visible
- [ ] Alerts configured

---

## 🔒 Phase 8 (Weeks 27–28) — Security

### Topics
- [ ] Secrets management
- [ ] RBAC
- [ ] Image scanning
- [ ] Least privilege
- [ ] Network policies
- [ ] TLS basics

### Tools
- [ ] Trivy
- [ ] Kyverno / OPA *(later)*

### Project
- [ ] Secure my cluster

---

## ☁️ Phase 9 (Weeks 29–32) — Cloud Kubernetes

### Choose one
- [ ] AWS EKS
- [ ] GKE
- [ ] AKS

### Topics
- [ ] Managed clusters
- [ ] IAM
- [ ] Load balancer
- [ ] Storage classes
- [ ] Costs

### Project
- [ ] Deploy backend to cloud Kubernetes

---

## 🏗️ Phase 10 (Weeks 33–36) — Real Portfolio Projects

| # | Project | Status |
|---|---------|--------|
| 1 | Food Delivery Backend on Kubernetes | ⬜ Not started |
| 2 | Payment Gateway Microservice Stack (Spring Boot + Kafka + PostgreSQL + K8s) | ⬜ Not started |
| 3 | Real-Time Tracking Platform (WebSocket + Redis + Kubernetes) | ⬜ Not started |
| 4 | Multi-Environment SaaS Deployment (dev / staging / prod namespaces) | ⬜ Not started |

---

## 🏅 Certification Path *(Optional but Strong)*

- [ ] **KCNA** — Cloud Native Computing Foundation (first)
- [ ] **CKAD** or **CKA** (then)

> Use certs as validation — not as my only skill proof.

---

## 📅 Weekly Routine

| Day | Activity |
|-----|----------|
| Mon–Fri | 1h learning + 1h hands-on |
| Saturday | Build project |
| Sunday | Review + publish progress |

---

## 📁 My GitHub Portfolio Must Show

- [ ] Kubernetes manifests
- [ ] Docker projects
- [ ] CI/CD pipelines
- [ ] Monitoring setup
- [ ] Cloud deployments
- [ ] Architecture diagrams
- [ ] Troubleshooting notes

---

## 📢 What to Post on LinkedIn / X Weekly

Every week, post:
- What I learned
- What broke
- How I fixed it
- Screenshot of cluster/project
- Repo link

---

## 💻 If on Low-End Hardware

Use these alternatives:
- **Kind** instead of Minikube
- Lightweight apps
- [Killercoda](https://killercoda.com) browser labs
- Play with Kubernetes sandboxes

---

## 🎯 Target Roles After 6 Months

- Junior DevOps Engineer
- Platform Engineer
- Cloud Engineer
- Kubernetes Support Engineer
- Backend + DevOps Hybrid Engineer

---

## 💡 My Personal Advantage

Since I already know backend development, my fastest path is:

> **Deploy backend systems repeatedly until DevOps becomes natural.**

Use real apps — not just nginx demos:
- Spring Boot
- PostgreSQL
- Redis
- Kafka
- Auth services
- Real APIs

This separates me from tutorial-only learners.

---

*Started: ___________  |  Target end date: ___________*
