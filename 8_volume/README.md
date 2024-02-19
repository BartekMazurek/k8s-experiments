# PersistentVolume & PersistentVolumeClaim example

## 1 - How to run
> kubectl apply -f volume.yaml

## 2 - Mount host path into minikube volume
> minikube mount $HOME/data:/data

## 3 - How to check if volume is created
> kubectl get pv

> kubectl get pvc

## 4 - Test volume
> kubectl exec -it ubuntu-pod --container='ubuntu-container' -- bash

> cd /home/data

> touch test.txt

> echo "It works!" > test.txt