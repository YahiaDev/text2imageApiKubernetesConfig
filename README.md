# text2imageWebKubernetesConfig
text2imageWebKubernetesConfig:


Ingress:
kubectl -n ingress-nginx port-forward svc/ingress-nginx-controller 8088:80
ArgoCD:
kubectl -n argocd port-forward svc/argocd-server 8080:80
