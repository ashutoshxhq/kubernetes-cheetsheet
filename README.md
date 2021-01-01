# Kubernetes
Repo for storing different configurations for k8s

## Creating a resource
This command can be used for creating a resource in kubernetes
```
kubectl create -f resource.yaml
```

## Updating a resource
This command can be used for updating a resource in kubernetes
```
kubectl replace -f resource.yaml
```

## Deleting a resource
This command can be used for deleting a resource in kubernetes
```
kubectl delete pod/replicaset/deployment RESOURCE_NAME
```

## Editing a resource
This command can be used for editing a resource in kubernetes
```
kubectl edit pod/replicaset/deployment RESOURCE_NAME
```