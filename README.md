# text2imageWebKubernetesConfig
text2imageWebKubernetesConfig:


build:
kustomize build overlays/dev | sed "s/:IMAGE_TAG/:0.0.2-SNAPSHOT/" > overlays/dev/manifest/manifest.yaml
Ingress:
kubectl -n ingress-nginx port-forward svc/ingress-nginx-controller 8088:80
ArgoCD:
kubectl -n argocd port-forward svc/argocd-server 8080:80
