# Simple nginx pod based on docker image example

## 1 - How to run
> kubectl apply -f pod.yaml

## 2 - How to check if pod is running
> kubectl get pods

## 3 - How to test nginx server
> kubectl port-forward nginx-pod 8080:80