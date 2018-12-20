# Flux GitOps Repo für NodeJS Hello World App

Der Weave Flux Operator wendet Änderungen an der Konfiguration an. Aktuelle Konfiguration:

- Kubernetes `demo` Namespace  (siehe [demo.yaml](namespaces/demo.yaml))
- Kubernetes Deployment für die [Hello World NodeJS App](https://github.com/HPrinz/gke-node-hello-world), verfügbar als Docker Image in Google Cloud (siehe [hellonode-dep.yaml](workloads/hellonode-dep.yaml))
- Kubernetes Service für die [Hello World NodeJS App](https://github.com/HPrinz/gke-node-hello-world), der dann via LoadBalancer öffentlich erreichbar ist (siehe [hellonode-svc.yaml](workloads/hellonode-svc.yaml))

Der Flux Operator commitet den Stand des Deployments nach Anwendung der Änderungen zurück in das Repository