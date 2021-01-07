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
Alternatively you could also use this command for update
```
kubectl apply -f resource.yaml
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

This command will extract the pod defination to a file and we can edit it and re create the pods.
```
kubectl get pod <pod-name> -o yaml > pod-definition.yaml
```

## Watching rollout status of deployment
This command can be used for watching rollout status of deployments.
```
kubectl rollout status deployment/DEPLOYMENT_NAME
```

## Rollout History of deployment
This command can be used for listing rollout history of the deployment.
```
kubectl rollout history deployment/DEPLOYMENT_NAME
```

## Undo Last Rollout of deployment
This command can be used to undo last rollout of the deployment.
```
kubectl rollout undo deployment/DEPLOYMENT_NAME
```

## Scale a deployment
This command can be used to scale a deployment.
```
kubectl scale deployment DEPLOYMENT_NAME --replicas=NUMBER_OF_REPLICAS
```
