# Kubernetes Learning Journey 🚀

This repository documents my journey learning Kubernetes fundamentals using Minikube.

## Environment Setup
- **OS**: macOS (Apple Silicon)
- **Kubernetes**: Minikube v1.36.0
- **kubectl**: v1.33.4
- **Container Runtime**: Docker Desktop

## Learning Path

### 1. Deployments vs Pods 📦
**Goal**: Understand why Deployments are preferred over bare Pods
- [x] Create a single Pod
- [ ] Create a Deployment
- [ ] Compare scaling behavior
- [ ] Test self-healing capabilities
- [ ] Practice rolling updates

**Key Concepts**:
- Pod lifecycle and limitations
- ReplicaSets and scaling
- Rolling updates and rollbacks
- Self-healing capabilities

### 2. Services 🌐
**Goal**: Learn how to expose applications within and outside the cluster
- [ ] ClusterIP Service (internal communication)
- [ ] NodePort Service (external access)
- [ ] LoadBalancer Service (cloud environments)
- [ ] Service discovery and DNS

**Key Concepts**:
- Service types and use cases
- Labels and selectors
- Endpoints and service discovery
- Port forwarding vs services

### 3. ConfigMaps & Secrets 🔐
**Goal**: Manage configuration and sensitive data properly
- [ ] Create and use ConfigMaps
- [ ] Environment variables from ConfigMaps
- [ ] Mount ConfigMaps as volumes
- [ ] Create and use Secrets
- [ ] Best practices for secrets

**Key Concepts**:
- Separating configuration from code
- Environment variables vs volume mounts
- Secret types and encoding
- Security considerations

### 4. Persistent Volumes 💾
**Goal**: Understand data persistence in Kubernetes
- [ ] Create PersistentVolumes
- [ ] Use PersistentVolumeClaims
- [ ] Deploy stateful applications
- [ ] Understand storage classes
- [ ] Data backup and recovery

**Key Concepts**:
- Stateful vs stateless applications
- Volume types and storage classes
- PV/PVC lifecycle
- Data persistence strategies

## Quick Commands Reference

```bash
# Cluster Management
minikube start                    # Start cluster
minikube stop                     # Stop cluster
minikube dashboard               # Open web UI
kubectl cluster-info             # Cluster information

# Pod/Deployment Management
kubectl get pods                 # List pods
kubectl get deployments         # List deployments
kubectl describe pod <name>      # Pod details
kubectl logs <pod-name>          # View logs
kubectl delete pod <name>        # Delete pod

# Services
kubectl get services             # List services
kubectl expose deployment <name> # Create service
kubectl port-forward <pod> 8080:80 # Port forward

# Apply/Create Resources
kubectl apply -f <file.yaml>     # Apply configuration
kubectl create -f <file.yaml>    # Create resource
kubectl delete -f <file.yaml>    # Delete resource
```

## Project Structure

```
kubernetes-learning/
├── 01-deployments-vs-pods/
│   ├── pod-example.yaml
│   ├── deployment-example.yaml
│   └── README.md
├── 02-services/
│   ├── clusterip-service.yaml
│   ├── nodeport-service.yaml
│   └── README.md
├── 03-configmaps-secrets/
│   ├── configmap-example.yaml
│   ├── secret-example.yaml
│   └── README.md
├── 04-persistent-volumes/
│   ├── pv-example.yaml
│   ├── pvc-example.yaml
│   └── README.md
├── examples/
└── docs/
```

## Progress Tracking

- [x] Environment setup (Minikube, kubectl, Docker)
- [x] First pod creation
- [x] Dashboard access
- [ ] Complete Deployments vs Pods section
- [ ] Complete Services section
- [ ] Complete ConfigMaps & Secrets section
- [ ] Complete Persistent Volumes section

## Resources

- [Kubernetes Official Documentation](https://kubernetes.io/docs/)
- [Minikube Documentation](https://minikube.sigs.k8s.io/docs/)
- [kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)

## Notes

Add your learning notes, observations, and "aha!" moments here as you progress through each section.