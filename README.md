## Add ArgoCd to K8s cluster
```bash
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
kubectl apply -n argocd -f https://raw.githubusercontent.com/Helga09/elephantSourcecode/master/argo.yaml
```
### Official documentation[https://argo-cd.readthedocs.io/en/stable/]
### Steps to install: `https://argo-cd.readthedocs.io/en/stable/getting_started/`

## Add Pixie to K8s cluster 

```bash
helm repo add pixie-operator https://artifacts.px.dev/helm_charts/operator
helm repo update
helm install pixie pixie-operator/pixie-operator-chart --set deployKey=<deploy-key-goes-here> --set clusterName=<cluster-name> --namespace pl --create-namespace
```
### Official documentation: `https://docs.px.dev/`
### Steps to install: `https://docs.px.dev/installing-pixie/install-schemes/helm`
