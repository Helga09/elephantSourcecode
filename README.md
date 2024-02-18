## Add ArgoCd to K8s cluster
```bash
kubectl create namespace argocd
kubectl apply -f https://raw.githubusercontent.com/Helga09/elephantSourcecode/master/argo.yaml  -n argocd
```
