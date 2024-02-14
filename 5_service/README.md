# Service with 3 nginx pod replicas

## 1 - How to run
> kubectl apply -f service.yaml

## 2 - How to check if service is running
> kubectl get service

## 3 - How to check communication between pods
> kubectl exec -it ubuntu-pod --container='ubuntu-container' bash

> curl http://nginx:8000