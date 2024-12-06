
# Kubernetes Deployement - 1

Simple javascript project deployment of a web application with a mongodb database for a javascript application.




## Deployment

Apply the each YAML configurations for the namespace.

```bash
change the working directory where the configuration files exists

cd k8demo
```
```bash
1.Applying mongo-config.yaml to the kubernetes cluster

kubectl apply -f mongo-config.yaml -n namespace  
```

```bash
2.Applying mongo-secret.yaml to the kubernetes cluster

kubectl apply -f mongo-secret.yaml -n namespace  
```

```bash
3.Applying mongo.yaml to the kubernetes cluster

kubectl apply -f mongo.yaml -n namespace  
```

```bash
4.Applying webapp.yaml to the kubernetes cluster

kubectl apply -f webapp.yaml -n namespace  

```

## Checking the Pods, deployements , Services and replicas for the given cluster

```bash
kubectl get all -namespace  
```

## Check each configuration
```bash

kubectl get configmap
```

```bash
kubectl get secret
```

## Description about the running Services
```bash
kubectl describe service service_name
```

## Log description of pod
```bash
kubectl get pods -n namespace
```





## 🔗 Links
Minikube installation: https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download



## Additional Information

In this deployement I used Rancher Desktop to use Docker and Kubernetes.

Docker image:

```bash
docker pull nanajanashia/k8s-demo-app
```
