# Simple ingress example with node port services

## 1 - How to run
> kubectl apply -f ingress.yaml

## 2 - Run ingress addons (will set ingress IP)
> minikube addons enable ingress

## 3 - Verify that ingress is running
> kubectl describe ingress app-ingress

## 4 - Verify that pods are running
> kubectl get pods

## 5 - Check service via NodePort
> minikube service nginx-service-1 --url

> minikube service nginx-service-2 --url

## 6 - Add ingress IP into /etc/hosts to set local domain
```console
sudo echo "[IP] app1.local" >> /etc/hosts
sudo echo "[IP] app2.local" >> /etc/hosts
```