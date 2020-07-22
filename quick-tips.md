## This file is intended for the purpose of quick tips that could save a lot of time during the exam. Please add more.

### Set alias for kubectl command

```bash
alias k=kubectl
```

### Find all the applicable shortnames for all the Kubernetes resources (Note: we have set the alias above)

```bash
k api-resources

#Check under the SHORTNAMES column for a particular resource.
#Example Service is svc, node is no, pod is po etc
k create svc nodeport my-svc --tcp=5678:8080
#service/my-svc created
```

### Find all resources in all the namespaces

```bash
# kubectl get pods --all-namespaces
k get po -A
```
