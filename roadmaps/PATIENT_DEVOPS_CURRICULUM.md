# 🏥 DevOps Curriculum — Patient Microservice Project
> Real project, real skills. Using my own codebase as the sandbox for every DevOps topic.
>
> **Path: Run it locally → Containerize it → Pipeline it → Deploy to K8s → Monitor it → Harden it → Present it**

---

## 🗂️ What My App Contains

| Service | Port | Notes |
|---------|------|-------|
| `patient-service` | `4000` | Resilience4j circuit breaker/retry, Actuator + Prometheus metrics |
| `auth-service` | `4005` | JWT security |
| `api-gateway` | `4004` | Gateway validation, Redis rate limiting |
| `billing-service` | `4001` | gRPC on port `9001` |
| `analytics-service` | `4002` | Kafka consumer |

**Infrastructure:**
- Kafka-based event flow
- Redis (gateway rate limiting)
- PostgreSQL/JPA (data services)
- JWT security (auth + gateway)
- Actuator + Prometheus metrics
- OpenAPI/Swagger
- `monitoring/prometheus.yml`
- Integration tests module

**Runtime flow:**
```
gateway → patient-service / auth-service
patient-service → billing-service (gRPC)
patient-service / billing-service → Kafka
analytics-service → consumes Kafka events
```

> ⚠️ Service-level `docker-compose.yml` files are currently empty — first task is to fix this.

---

## 📊 Overall Progress

| Month | Focus | Status |
|-------|-------|--------|
| Month 1 | Repo mastery, Linux, Docker, local execution | ⬜ Not started |
| Month 2 | CI/CD for multi-service Spring Boot | ⬜ Not started |
| Month 3 | Kubernetes for this exact architecture | ⬜ Not started |
| Month 4 | Cloud + Infrastructure as Code | ⬜ Not started |
| Month 5 | Observability, reliability, production ops | ⬜ Not started |
| Month 6 | Security, hardening, scaling, portfolio | ⬜ Not started |

---

## 📅 Month 1 — Repo Mastery, Linux, Docker, Local Execution

> **Goal:** Get the whole project running cleanly on my machine.

### Week 1 — Repo Audit

- [ ] Map every service and its role
- [ ] Identify ports, dependencies, databases, topics, gRPC links, and auth flow
- [ ] Document the full runtime flow (gateway → patient/auth, patient → billing via gRPC, patient/billing → Kafka, analytics consumes events)

---

### Week 2 — Docker Fundamentals on the Real Project

- [ ] Write one Dockerfile per service
- [ ] Optimize Java builds with multi-stage images
- [ ] Standardize JVM options and health checks
- [ ] Run each service individually with Docker

---

### Week 3 — Compose the Full Stack

- [ ] Create a real top-level `docker-compose.yml`
- [ ] Include PostgreSQL, Kafka, Redis, Zookeeper/Kraft
- [ ] Bring up the entire system with one command
- [ ] Validate service-to-service networking

---

### Week 4 — Local Debugging Discipline

- [ ] Logs
- [ ] Env vars
- [ ] Port conflicts
- [ ] Startup ordering
- [ ] Health endpoints
- [ ] Failure simulation

### ✅ Month 1 Deliverable
- [ ] Fully containerized local environment for the patient platform

---

## 📅 Month 2 — CI/CD for a Multi-Service Spring Boot System

> **Goal:** Build pipelines that test, package, scan, and publish every service.

### Week 5 — Pipeline Basics

- [ ] Build each service in CI
- [ ] Run unit tests
- [ ] Run integration tests
- [ ] Cache Maven dependencies

---

### Week 6 — Quality Gates

- [ ] Code style checks
- [ ] Test coverage thresholds
- [ ] Fail builds on broken tests
- [ ] Verify generated protobuf/gRPC artifacts

---

### Week 7 — Image Pipelines

- [ ] Build Docker images for all services
- [ ] Tag by commit SHA and version
- [ ] Push to a registry

---

### Week 8 — Release Flow

- [ ] Create dev/staging/release pipelines
- [ ] Implement rollback strategy
- [ ] Version the patient platform as a release train

### ✅ Month 2 Deliverable
- [ ] CI/CD pipeline that builds and publishes the whole stack automatically

---

## 📅 Month 3 — Kubernetes for This Exact Architecture

> **Goal:** Turn the project into a production-style Kubernetes deployment.

### Week 9 — Core K8s Objects

- [ ] Pods
- [ ] Deployments
- [ ] Services
- [ ] ConfigMaps
- [ ] Secrets
- [ ] Namespaces

---

### Week 10 — Deploy the Services

- [ ] `patient-service`
- [ ] `auth-service`
- [ ] `billing-service`
- [ ] `analytics-service`
- [ ] `api-gateway`

---

### Week 11 — Networking and Traffic

- [ ] Ingress controller
- [ ] Gateway routing
- [ ] Internal cluster DNS
- [ ] Service discovery
- [ ] Readiness probes
- [ ] Liveness probes

---

### Week 12 — State and Messaging

- [ ] PostgreSQL deployment strategy
- [ ] Kafka deployment strategy
- [ ] Redis deployment strategy
- [ ] Persistent volumes where needed

### ✅ Month 3 Deliverable
- [ ] Working Kubernetes deployment for the full platform

---

## 📅 Month 4 — Cloud + Infrastructure as Code

> **Goal:** Build the infrastructure around the app like a real platform engineer.

### Week 13 — Cloud Foundations

- [ ] VPC/networking
- [ ] Subnets
- [ ] Security groups
- [ ] IAM
- [ ] Load balancers

---

### Week 14 — Terraform Basics

- [ ] Declare infrastructure
- [ ] Manage variables
- [ ] Outputs
- [ ] Remote state

---

### Week 15 — Terraform for the Patient Platform

- [ ] Provision network
- [ ] Provision Kubernetes cluster
- [ ] Provision registry
- [ ] Provision database and supporting services

---

### Week 16 — Environment Management

- [ ] dev/staging/prod separation
- [ ] Reusable modules
- [ ] Secret handling
- [ ] Environment-specific values

### ✅ Month 4 Deliverable
- [ ] Infrastructure as code for the platform — no click-ops

---

## 📅 Month 5 — Observability, Reliability, and Production Operations

> **Goal:** See, measure, and operate the system.

### Week 17 — Metrics

- [ ] Expand Prometheus scraping beyond `patient-service`
- [ ] Expose metrics for all services
- [ ] Define useful service-level metrics

---

### Week 18 — Dashboards

- [ ] Grafana dashboard: requests, errors, latency, throughput
- [ ] JVM dashboards
- [ ] Kafka consumer health
- [ ] gRPC call visibility

---

### Week 19 — Logging

- [ ] Structured logs
- [ ] Correlation IDs
- [ ] Centralized log collection
- [ ] Trace request flow across gateway → patient → billing → analytics

---

### Week 20 — Reliability Engineering

- [ ] Circuit breakers
- [ ] Retries
- [ ] Timeouts
- [ ] Backpressure thinking
- [ ] Incident runbooks
- [ ] Postmortems

### ✅ Month 5 Deliverable
- [ ] Observable system with dashboards and failure-handling patterns

---

## 📅 Month 6 — Security, Hardening, Scaling, and Portfolio

> **Goal:** Make the project interview-ready and production-shaped.

### Week 21 — Security

- [ ] JWT hardening
- [ ] Secret management
- [ ] Least privilege
- [ ] Container scanning
- [ ] Dependency scanning
- [ ] API protection

---

### Week 22 — Scaling

- [ ] Horizontal Pod Autoscaling (HPA)
- [ ] Resource requests and limits
- [ ] Kafka scaling considerations
- [ ] Cache tuning for Redis
- [ ] Gateway rate-limiting strategy

---

### Week 23 — Production Hardening

- [ ] Blue/green or rolling deploys
- [ ] Rollback drills
- [ ] Backup strategy
- [ ] Disaster recovery basics
- [ ] Upgrade strategy for services

---

### Week 24 — Portfolio and Interviews

- [ ] Architecture diagram
- [ ] README rewrite
- [ ] Deployment guide
- [ ] DevOps case study for this project
- [ ] Interview questions based on my own system

### ✅ Month 6 Deliverable
- [ ] Portfolio-ready DevOps case study built from my actual repo

---

## 🔨 First 3 Practical Upgrades to Do on This Repo

- [ ] **1. Create a proper root-level orchestration layer** — one `docker-compose.yml` or one environment directory for the full stack
- [ ] **2. Standardize service packaging** — one Dockerfile pattern per service, with consistent runtime variables
- [ ] **3. Expand observability** — Prometheus currently only targets `patient-service`; extend metrics to the rest of the stack

---

## 🧰 DevOps Topics Covered via This Project

| Topic | Applied To |
|-------|-----------|
| Docker | All services |
| CI/CD | The full repo |
| Kubernetes | Full stack deployment |
| Terraform | Cloud infrastructure |
| Prometheus/Grafana | Observability across all services |
| Kafka + gRPC | Distributed system realism |
| JWT + Gateway | Platform security |
| PostgreSQL + Redis | Stateful service operations |

---

*Started: ___________  |  Target end date: ___________*
