Create Secret: 

kubectl create ns wp-prod

kubectl create secret generic mysql-pass --from-literal=password=supersecretpass1234 -n wp-prod

k apply -f examples/mysql-deployment.yaml -n wp-prod

helm upgrade --install  demo-wp chart/wordpress -n wp-prod  --debug --dry-run 