# start version 

```
minikube start --kubernetes-version=v1.23.2
```

```
minikube config defaults kubernetes-version
```


# KIEM TRA VERSION HPA

```
kubectl api-versions | grep autoscaling
```




# KIEM TRA EVENT
```
`kubectl get events -n dev-npc`

```

```
kubectl delete events --all -n dev-npc
```

```yaml
  kubectl get deployment metrics-server -n kube-system
```



# KIEM TRA METRICS
https://www.linuxtechi.com/how-to-install-kubernetes-metrics-server/
```
kubectl top pods
```

```
kubectl get pods -n kube-system
```


# TAO SERIVCE ACCOUNT
```
1. `kubectl create serviceaccount dev-npc-authentication-api-sa -n dev-npc`
```


# GAN NODE VOI LABEL 
```
kubectl label node minikube env=int
node/minikube labeled
```

```
kubectl get node minikube --show-labels
```
