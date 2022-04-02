kubectl create ns argocd

kubectl apply -f https://raw.githubusercontent.com/argoproj/argo-cd/v2.3.3/manifests/install.yaml -n argocd