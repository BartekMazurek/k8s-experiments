# 2 separate namespaces with different pods

## 1 - How to run
> kubectl apply -f namespace.yaml

## 2 - How to check namespaces
> kubectl get namespace

## 3 - How to check communication between pods in different namespaces
> kubectl exec -it ubuntu-pod --container='ubuntu-container' -- bash

> curl http://nginx.web.svc.cluster.local:8000