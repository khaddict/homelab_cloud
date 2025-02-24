# My ☁️ Homelab

## 1) Introduction 👨🏻‍💻

The goal of this GitHub repository is to deploy ArgoCD applications to my Kubernetes cluster.

## 2) ArgoCD 🐙

ArgoCD is a declarative, GitOps continuous delivery tool for Kubernetes. It automates the deployment and management of applications, ensuring that the deployed state in the cluster matches the configuration stored in a Git repository. With features like automated sync, rollback, and monitoring, ArgoCD simplifies Kubernetes application management and provides a robust way to manage infrastructure as code.

## 3) File structure 🗂️

```
├── apps
│   ├── app1
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   │   ├── app1_namespace.yaml
│   │   │   └── app1_pod.yaml
│   │   └── values.yaml
│   └── app2
│       ├── Chart.yaml
│       ├── templates
│       │   ├── app2_deployment.yaml
│       │   ├── app2_ingressroute.yaml
│       │   ├── app2_secret.yaml
│       │   ├── app2_serviceaccount.yaml
│       │   ├── app2_service.yaml
│       │   └── app2_tls.yaml
│       └── values.yaml
├── argocd
│   ├── Chart.yaml
│   ├── templates
│   │   ├── app1
│   │   │   └── app1-app.yaml
│   │   └── app2
│   │       └── app2-app.yaml
│   └── values.yaml
├── homelab-app-of-apps.yaml
└── README.md
```

## 4) What does it look like?

### a) The ArgoCD applications deployed:
![image](https://github.com/user-attachments/assets/920472a7-60ff-4647-b69b-ddaeb8208d43)

### b) The khaddict.com application deployment:
![image](https://github.com/user-attachments/assets/73e28853-7c15-4c31-9dc1-87ac945330e6)
