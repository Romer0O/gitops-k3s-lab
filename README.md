# 🚀 GitOps CI/CD Lab: K3s, FastAPI, PostgreSQL, Helm & ArgoCD

A production-grade, cloud-native GitOps pipeline implemented locally on WSL2 using **K3s**, **ArgoCD**, **Helm**, and **FastAPI** connected to a persistent **PostgreSQL** database.

---

## 🏗 Architecture & Tech Stack

* **Orchestration:** K3s (v1.36.4) on WSL2
* **GitOps Continuous Delivery:** ArgoCD
* **Package Management:** Helm Charts (`myapp-chart`)
* **Backend Application:** FastAPI (Python) with database connectivity endpoint
* **Database:** PostgreSQL with PersistentVolume (PVC)
* **Ingress Controller:** Traefik (Path-based routing)

---

## 📂 Project Structure

```text
gitops-k3s-lab/
├── myapp-chart/              # Custom Helm Chart
│   ├── templates/            # Kubernetes Manifests (Deployment, Service, Ingress, PVC)
│   └── values.yaml           # Configuration values (Image tags, replicas, etc.)
└── README.md
