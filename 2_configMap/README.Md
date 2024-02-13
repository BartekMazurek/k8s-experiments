# ConfigMap

## 1 - How to run
> kubectl apply -f config_map.yaml

## 2 - How to check variables
> kubectl -it exec nginx-app --container='nginx-app' -- bash -c 'echo $APP_NAME'

or

> kubectl describe pod nginx-app
