#How to connect to the cluster
connect to the kubernetes cluster like this: az aks get-credentials --admin --name showcase-dev --resource-group showcase-dev-k8s

# Access Argocd
-  Public IP = "kubectl -n argocd get svc argocd-server"
-  Password= "kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d"