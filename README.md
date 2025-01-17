podman machine set --cpus=4 --memory=4096
minikube start --driver=podman --container-runtime=containerd --cpus 4 --memory 3896 
kubectl port-forward  -n argocd service/argocd-server 8080:443
kubectl get secret -n argocd argocd-initial-admin-secret -o yaml
