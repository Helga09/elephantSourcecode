## Add ArgoCd to Kubernetes cluster
```bash
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
kubectl apply -n argocd -f https://raw.githubusercontent.com/Helga09/elephantSourcecode/master/argo.yaml
```
