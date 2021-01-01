# Kubernetes
This repo contains sample files and commands for managing a kubernetes cluster. 

## Listing Resources
This command can be used for listing resources in kubernetes
```
kubectl get pods/replicasets/deployments/services
```

For listing all resources
```
kubectl get all
```

This command can be used for detailed listing of resources in kubernetes
```
kubectl get pods/replicasets/deployments/services -o wide
```

## Describe a resource
This command can be used for describing a resource in kubernetes
```
kubectl describe pod/replicaset/deployment RESOURCE_NAME
```

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