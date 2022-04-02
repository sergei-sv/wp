Create Secret: 

kubectl create secret generic mysql-pass --from-literal=password=supersecretpass1234

kubectl port-forward svc/wordpress 8080:80