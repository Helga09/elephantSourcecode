## Add ArgoCd to K8s cluster
```bash
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml,https://raw.githubusercontent.com/Helga09/elephantSourcecode/master/argo.yaml
```
